# Linear regression with one variable



## Model representation

In supervised learning , we are given the "right answer" for each example in the data.

**m** = Number of training examples

**x's** = "input" variable/ features

**y's** = "output" variable/ "target" variable

We use hypothesis  to map x's to y's:
$$
h_{\theta}(x)=\theta_{0}+\theta_{1} x
$$
**$h$  = hypothesis**

**$\theta_{i}$ = parameters**

**But how to choose $\theta_{i}$ ? **

We should choose $\theta_{0},\theta_{1}$so that $h_{\theta}(x)$ is close to $y$ for our training examples $(x,y)$

We use **cost function** to do that.



## Cost Function

We can measure the accuracy of our hypothesis function by using a **cost function**. This takes an average difference (actually a fancier version of an average) of all the results of the hypothesis with inputs from x's and the actual output y's.

**Cost Function:**
$$
J(\theta_0, \theta_1) = \dfrac {1}{2m} \displaystyle \sum _{i=1}^m \left ( \hat{y}_{i}- y_{i} \right)^2 = \dfrac {1}{2m} \displaystyle \sum _{i=1}^m \left (h_\theta (x_{i}) - y_{i} \right)^2
$$
To break it apart, it is $\frac{1}{2}\bar{x}$ where $\bar{x}$ is the mean of the squares of $h_\theta (x_{i}) - y_{i}$ , or the difference between the predicted value and the actual value.

This function is otherwise called the "Squared error function", or "Mean squared error". The mean is halved $\left(\frac{1}{2}\right)$ as a convenience for the computation of the gradient descent, as the derivative term of the square function will cancel out the $\frac{1}{2}$ term. 

**Goal: minimize function $J$** 



## Gradient Descent

$J\left(\theta_{0}, \theta_{1}\right)$ is a function of the parameter $\theta_{0}, \theta_{1}$

In order to get  $\min _{\theta_{0}, \theta_{1}} J\left(\theta_{0}, \theta_{1}\right)$ , we should:

- Start with some $\theta_{0}, \theta_{1}$
- Keep changing $\theta_{0}, \theta_{1}$ to reduce $J\left(\theta_{0}, \theta_{1}\right)$ until we hopefully end up at a minimum



### Gradient descent algorithm

repeat until convergence:
$$
\theta_j := \theta_j - \alpha \frac{\partial}{\partial \theta_j} J(\theta_0, \theta_1)
$$
where

j=0,1 represents the feature index number.

At each iteration j, one should simultaneously update the parameters $\theta_1, \theta_2,...,\theta_n$. Updating a specific parameter prior to calculating another one on the $j^{(th)}$ iteration would yield to a wrong implementation.



**Learning Rate $\alpha$ **: the size of each step is determined by parameter $\alpha$, which is called learning rate.

- if $\alpha$ is too small, gradient descent can be slow.
- if $\alpha$ is too large, gradient descent can overshoot the minimum. it may fail to converge, or even diverge.



**Update $\theta_{0}, \theta_{1}$ simultaneously.**



### "Batch" Gradient descent

"Batch": each step of gradient descent uses all the training examples.









