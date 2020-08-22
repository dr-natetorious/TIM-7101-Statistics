# Readings

## Regression analysis by example (2012)

Chatterjee, S., & Hadi, A. S. (2012). Regression analysis by example. Hoboken, New Jersey: John Wiley & Sons, Inc. [ProQuest](https://ebookcentral.proquest.com/lib/ncent-ebooks/detail.action?docID=918623).

### 1: What is regression analysis

Regression analysis is a common statistical approach for modeling the relationship of multiple variables.  It attempts to approximate a function that uses the parameter set to come to some known outcome.  After estimating this function, researchers can predict behaviors in other groups.

![regression_analysis_process.png](regression_analysis_process.png)

### 2: Simple Linear Regression

Measuring the `direction` and `strength` of a relationship requires calculating the `covariance` and `correlation coefficienct`.  After determining these values it can be useful to also determine `standard error rate` and the `confidence interval`, which are measurements of accuracy.

### 4: Regression diagnostics: detection of model violations

There are several risks to regression analysis that produce overfitting or erroneous solutions.

Assumption of...

- ... `linearity` that the model is simple versus hihgly dimensional
- ... `independently and identically distributed` (iid) normal random variables
- ... predictor variables are (a) non random (b) measured without error and (c) linearly independent (`collinearity`)
- ... observations are equally reliable and approximately equal influence

One strategy for proving or disproving these assumptions is to graphically present the data.

- Detect errors in the data
- Recognize patterns (e.g., clusters, outliers, gaps)
- Explore relationships
- Discover new phenomena
- Confirm or negate assumptions
- Assess adequancy of fitting
- Suggest remedial actions (e.g., transform, redesign, or additional collection)
- Enhance numerial analyses in general

Another strategy is to measure the influence of an individual point, using something like `Cook's distance`; which removes the `ith` data point then recalculates the regression line.  Similarly, Welsch and Kuh (1977) propose `DFITS` to derive a _difference in fit scaled_.  Hadi (1992) uses a _normalized residual_ to discover outliers in parameters and data points.

### 6: Transformation of variables

This chapter looks really useful.  I will come back to this after lunch.

## What is the proper way to apply the multiple comparison test (2018)

Sangseok Lee, & Dong Kyu Lee. (2018). What is the proper way to apply the multiple comparison test? Korean Journal of Anesthesiology, 71(5), 353–360. [https://doi-org.proxy1.ncu.edu/10.4097/kja.d.18.00242](https://doi-org.proxy1.ncu.edu/10.4097/kja.d.18.00242). [MultipleComparisonTests.pdf](MultipleComparisonTests.pdf).

## Anova and ancova: A glm approach (2012)

Rutherford, A. (2012). Anova and ancova: A glm approach. Hoboken, New Jersey: John Wiley & Sons, Inc. [ProQuest](https://ebookcentral.proquest.com/lib/ncent-ebooks/detail.action?docID=1011369).

### 1: Introduction to General Linear Models: Regression, Analysis of Variance, and Analysis of Covariance

### 2: Traditional and GLM Approaches to Independent Measures Single Factor ANOVA Designs

### 3: Comparing Experimental Condition Means, Multiple Hypothesis Testing, Type 1 Error, and a Basic Data Analysis Strategy

### 4: Measures of Effect Size and Strength of Association, Power, and Sample Size

### 5: GLM Approaches to Independent Measures Factorial Designs

## Exploring data in R (2018)

Shaughnessy, A., Prener, C., & Hasenmueller, E. (2018). Exploring data in R. [GitHub](https://shaughnessyar.github.io/driftR/articles/ExploringData.html).  [ExploringDataR.pdf](ExploringDataR.pdf).

## How to Select Appropriate Statistical Tests in Scientific Articles (2016)

Trajkovski, V. (2016). How to Select Appropriate Statistical Tests in Scientific Articles. Journal of Special Education & Rehabilitation. 7(3/4), 5–28. [https://doi-org.proxy1.ncu.edu/10.19057/jser.2016.7](https://doi-org.proxy1.ncu.edu/10.19057/jser.2016.7). [SelectStatisticalTests.pdf](SelectStatisticalTests.pdf).
