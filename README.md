# Leukemia Gene Expression Classification

Leukemia describes a group of blood disorders characterized by the dysfunctional production and development of lymphocytes, a type of white blood cell.

In this notebook, 2 different models are provided to solve multiclass classification problem on [leukemia gene expression dataset](https://www.kaggle.com/datasets/brunogrisci/leukemia-gene-expression-cumida) from [Curated Microarray Database (CuMiDa)](https://sbcb.inf.ufrgs.br/cumida)[^footnote].

The common challenge in gene expression arrays is that they violate the assumption that the number of samples is higher than the number of predictors (*p >> n*). Therefore, *Naive Bayes Classifier* and *Support Vector Machines* will be used as model algorithms, which perform well on such data most of the time. The dimensionality of the original dataset will be reduced by decomposing it into principal components and keeping the principal components that explain the 90% of the variance. The reduced version of the data will be feeding the Support Vector Classifier. 
