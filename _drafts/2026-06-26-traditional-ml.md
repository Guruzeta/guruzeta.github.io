---
title: "Quantifying uncertainty in xgboost using conformal prediction"
date: 2026-06-03
excerpt: "How do we quantify prediction uncertainty of conventional ML methods?"
tags: [meta]
permalink: /blog/xgboost-conformal/
---



Today we're documenting a well-encountered problem in traditional ML methods - the problem of attaching variance to pointwise estimates. Statistical learning methods, like linear regression or xgboost give pointwise estimates (by learning a map $f:\text{feature space}\to \text{output space}$), but assigning variance or confidence bounds to these variables isn't native in these methods. While other metrics like RMSE/correlation values can give a sense of the global-fit correctness of the methods, in a variety of applications it is more relevant to output a local distribution $\mathcal{P}(f(x))$ instead of pointwise $f(x)$. 



One relevant example that I'm currently dealing with involves predicting the output of a laser-plasma accelerator (more on that on a later post) at various points along the beamline (i.e. the setup involves stacking multiple complex components one after another and involves tedious tuning of parameters to achieve optimal performance), so the operator at any point along the beamline would ideally want a neural network to output predicted settings for their tuning knob at that point and then also a spread, to assess whether and how much to trust the ML output. This highlights another aspect of the conformal prediction usage - it is useful for **high-risk environments** where the cost of NN's incorrect predictions are high. In the case of particle accelerators, this implies the NN recommending incorrect beamline settings which could potentially damage the hardware and would be quite expensive to ameliorate. 
Moreover, practically, if the optimal settings lie quite far from the predicted distribution (e.g. $>3\sigma$ for gaussian/near gaussian outputs), then the neural network would require retraining, hence it also informs the modeler when to discard/re-train their model. 



So today we'll document how to use xgboost alongside conformal predictions to make uncertainty quantifications in our ML model. In doing that, we will also ask a series of engineering questions:-

1. How does this method work when the data size scales i.e. 10x'ed or 100x'ed for example?
2. How much compute is required to make this run? (Practically when to use local MacBook/ask for cloud credits)
3. How to estimate the training/inference time?
4. How interpretable are these methods? i.e. if a spread is given, then what do we tune or change or if there are concrete strategies to reduce the variance in these methods

---

What is xgboost?

**gradient boosting** with

1. Subsequent learning from residuals, minimizing residual losses, 2nd order expansion of the loss function (this time a functional expansion and not simple taylor series)
2. explicit regularization to limit the complexity of the tree
3. shrinkage+column subsampling
4. sparsity aware split finding
5. cache aware histogram algorithm

---

What is gradient boosting?

Boosting refers to the process of combining several weak learners to create a stronger predictor.

A weak learner is a learner that is slightly better than just guessing (i.e. predicting the mean in case of regression, attributing classes by random chance for classifying) and makes lots of mistakes on its own. However, it offers simplicity and easier training/inference, so it is a better starting point than deep NNs or complex MLPs. For example, a shallow decision tree.

Boosting involves combining several such weak-learners to generate a an ensemble of trees that are combined to predict the output at much higher accuracy than each individual tree ever could. (Aside: it might be possible to boost a sequence of MLPs, but you can do that itself by using more parameters. Also I imagine boosting a bunch of MLPs is much slower and compute intensive than xgboost)

gradient boosting involves:

1. Start with a simple prediction
2. Look at the errors
3. Then train another predictor on those errors/residuals
4. Add the new model to the existing model as a correction
5. Keep iterating on this process until we either reach the noise floor or overfit to the noise (so do regularization then)

Mathematically, gradient boosting is a perturbative expansion of a strong predictor in terms of several weak predictors as a taylor series
$$
\hat{f}(x) = f_0(x)+\eta f_1(x) + \eta f_2(x) + \dots + \eta f_M(x)
$$
So the gradient-descenting occurs in function space. For xgboost purposes, it every correction $f_k(x)$ is a decision tree. 



Also another thing - it is called "boosting" because it "boosts" the net model's performance by combining several weak learners. 

---

### Decision tree

A decision tree predicts the output at a given input by querying a sequence of yes/no questions the input feature questions and depending on the answers, it outputs the value of the the function at a given point. For example for computing $f(x=3)$, it'll proceeds by first checking $x \lessgtr 5 $ for example and then $x\lessgtr 1$ and then so on.  



---

### Conformal prediction

Modern neural nets are systematically overconfident : https://proceedings.mlr.press/v70/guo17a/guo17a.pdf

They can be miscalibrated, 







#### Confidence intervals





---

More stuff to write about

- Tea-leaves in loss and training:
  - https://cs231n.github.io/neural-networks-3/?utm_source=chatgpt.com#eval
- https://d2l.ai/chapter_linear-regression/generalization.html?utm_source=chatgpt.com

