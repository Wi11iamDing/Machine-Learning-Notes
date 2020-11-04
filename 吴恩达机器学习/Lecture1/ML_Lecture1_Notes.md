# Introduction



## What is machine learning?

### Machine Learning definition:

- Arthur Samuel(1959). **Machine Learning**: Field of study that gives computers the ability to learn without being explicitly programmed.

- **机器学习**：无需对计算机明确编程也能让其具备学习能力的一项研究领域

  

- Tmo  Mitchell(1998).Well-posed Learning Problem: A computer program is said to learn from **experience E** with respect to some **task T** and some **performance measure P**, if its performance on T, as measured by P, improves with experience E.

- 良好的学习问题：如果一个计算机程序问题在**任务T**上的性能由**P**测度，根据**经验E**改善，那么这个计算机程序问题可以说是从一些任务T和性能指标P中学习经验E。

### Machine Learning algorithms:

- Supervised learning
- Unsupervised learning
- Other: Reinforcement learning, Recommender systems



## Supervised Learning

In supervised learning, we are given a data set and already know what our correct output should look like, having the idea that there is a relationship between the input and the output.(**Right Answer Given**)

在有监督学习中，我们被给定一个已知正确输出的数据集，并且认为在数据集的输入和输出之间存在某种关系。（**已知正确的输出**）



Supervised learning problems are categorized into "regression" and "classification" problems.

-  In a regression problem, we are trying to predict results within a continuous output, meaning that we are trying to map input variables to some **continuous function**. 
-  Housing price prediction
-  In a classification problem, we are instead trying to predict results in a discrete output. In other words, we are trying to map input variables into **discrete categories**.
   -  Breast cancer (malignant or benign) classification

有监督学习可以分为回归和分类两个问题：

- 在回归问题中，将输入变量映射到一个连续的回归输出。
  - 房价预测
- 在分类问题中，将输入变量映射到一个离散的分类输出。
  - 乳腺癌分类（恶性还是良性）





## Unsupervised Learning

Unsupervised learning allows us to approach problems with little or no idea what our results should look like. We can derive structure from data where we don't necessarily know the effect of the variables.

We can derive this structure by clustering the data based on relationships among the variables in the data.

With unsupervised learning there is **no feedback** based on the prediction results.

无监督学习可以允许在不知道具体结果的情况下处理问题。我们可以从数据中获得结构，而不必要知道变量的影响。

我们可以基于数据中变量之间的相互关系，通过对数据进行聚类分析，从而了解数据的结构。

无监督学习中，没有基于预测结果的反馈。