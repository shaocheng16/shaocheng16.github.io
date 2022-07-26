---
layout: post
title:  "Mechine learning: 01"
data: Sat 22 Jul 2017 03:14:20 PM EDT
categories: research
---
- The problem of searching for patterns in data is fundamental one and has a long and successful history. 
- The field of **pattern recognition** is concerned with the automatic discovery of _regularities in data_ through the use of **computer algorithms** and with the use of these regularities to take action such as classifying the data into different categories. 
- In mechine learning, a training set is used to tune the parameters of an adaptive model. 
- In most applications, the original training sets are preprocessed to transform them into some new space of variables where, it is hoped, the pattern recognition problem will be easier to solve
    + this pre-processing stage is sometimes also called feature extraction. 

---

### Types of mechine learning:
- supervised learning 
    +  classification problem 
- unsupervised learning
    + to discover groups of similar examples within the data (clustering)
    + determine the distribution of data within the input space (density estimation)
    + project the data from high-dimensional space down to low dimensions for the purpose of *visualization*.
- reinforcement learning
    + to find suitable actions to take in a given situation in order to maximize a reward.   
    + the learning algorithm is not given examples of optimal outputs, in contrast to supervised learning, but must instead discover them by a process of trial and error. 

---

### Example: polynomial Curve Fitting
- Data generated for this example:
    + sin(2\pi x) with random noise
    + the data sets process an underlying regularity, which we wish to learn, but that individual observations are corrupted by random noise. 
    - the noise might arise from intrinsically stochastic processes such as radioactive decay but more typically is due to there being sources of variability that are themselves unobserved. 
- Training set:
    + N observations of x: X=(x1, x2, ... xN)^T
    + the corresponding observations: T= (t1, t2, ..., tN)^T
- The goal is to exploit this training set in order to make prediction of the value t^ of the target variable for some new value x^ of the input variable. 
- The values of the coefficients will be determined by fitting the polynomial to the training data. 
    - This can be done by minimizing an error function that measures the misfit between the function y(x,W), for any given value w, and the training set data points. 
- The remain problem is the choosing the order M of the polynomial, and this will turn out to be an example of an important concept called model comparison or modelselection. 
    + More flexible polynomials with larger values of M are becoming **increasingly tuned to the random noise on the target values**.
    + For a given model complexity, the over-fitting problem become less severe as the the size of the data set increase.
    + *the number of parameters is not necessarity the most appropriate measure of model complexity.*
    - The over-fitting problem can be understood as a general property of maximum likelihood. 
    + The over-fitting problem can be avoided by adopting a Bayesian approach. 
    + in a Bayesian model, the *effective* number of parameters adapts automatically to the size of the data set. 
- One technique that is often used to control the over-fitting problem:
    + adding a penalty term to the error function in order to discourage the coefficients from reaching large values. 
- Take home message: if we are trying to solve a practical applications using the approach of minimizing an error function, we would have to find a way to determine a suitable value for the model complexity. 

---

### Probability theory
- A key concept in pattern recognition is that of uncertainty:
    + noise on measurement
    + finite size of data sets

Probability theory provides a consistent framework for the quantificaion and manipulation of uncertainty and forms one of the central fundations for pattern recognition. 
- It allows us to make optimal predictions given all the information available to us, even though that information may be incomplete or ambiguous. 

#### Bayesian probabilities
- Classsical or frequentist interpretation of probability is based on the frequencies of random, repeatable events. 
- **Bayesian view**: probabilities provide a quantification of uncertainty. 
- Bayes' theorem was used to convert a prior probability into a posterior probability by incorporating the evidence provided by the observed data. 
- The Bayesian framework has its origins in the 18th century, however, the practical application of Bayesian methods was for a long time severely limited by the difficulties in carrying through the full Bayesian procedure, particularly the need to marginalized over the whole of parameter space.







