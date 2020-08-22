# Readings

## Regression analysis by example (2012)

Chatterjee, S., & Hadi, A. S. (2012). Regression analysis by example. Hoboken, New Jersey: John Wiley & Sons, Inc. [ProQuest](https://ebookcentral.proquest.com/lib/ncent-ebooks/detail.action?docID=918623).

> Praise for the Fourth Edition: "This book is . . . an excellent source of examples for regression analysis. It has been and still is readily readable and understandable." --Journal of the American Statistical Association Regression analysis is a conceptually simple method for investigating relationships among variables. Carrying out a successful application of regression analysis, however, requires a balance of theoretical results, empirical rules, and subjective judgment. Regression Analysis by Example, Fifth Edition has been expanded and thoroughly updated to reflect recent advances in the field. The emphasis continues to be on exploratory data analysis rather than statistical theory. The book offers in-depth treatment of regression diagnostics, transformation, multicollinearity, logistic regression, and robust regression. The book now includes a new chapter on the detection and correction of multicollinearity, while also showcasing the use of the discussed methods on newly added data sets from the fields of engineering, medicine, and business. The Fifth Edition also explores additional topics, including: Surrogate ridge regression Fitting nonlinear models Errors in variables ANOVA for designed experiments Methods of regression analysis are clearly demonstrated, and examples containing the types of irregularities commonly encountered in the real world are provided. Each example isolates one or two techniques and features detailed discussions, the required assumptions, and the evaluated success of each technique. Additionally, methods described throughout the book can be carried out with most of the currently available statistical software packages, such as the software package R. Regression Analysis by Example, Fifth Edition is suitable for anyone with an understanding of elementary statistics.

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

When examining the `mean` of multiple groups it is often useful to perform an `analysis of variance (ANoVA)`.  These strategies (e.g., Tukey, Newman-Keuls, Bonferroni, Dunneet, Scheffe, ...) compare the similarity of two or more distributions.

The various methods attempt to determine the statistical significance or `P-value (probability value)`-- or likelyhood of an extreme value occurring.  One challenge with measuring the p-value comes from `alpha inflation` which means that the same group is measured over-and-over resulting in _greater confidence despite no additional evidence_.  Comparisons typically use a single-step or stepwise procedure, which [adds or removes parameters](https://youtu.be/AdFT17sq53s) to determine which features are most important.

> Many research designs use numerous sources of multiple comparison, such as multiple outcomes, multiple predictors,
subgroup analyses, multiple definitions for exposures and outcomes, multiple time points for outcomes (repeated measures), and multiple looks at the data during sequential interim monitoring. Therefore, multiple comparisons performed in a previous situation are accompanied by increased type I error problem, and it is necessary to adjust the P value accordingly.

![mct_strategies.png](mct_strategies.png)

## Anova and ancova: A glm approach (2012)

Rutherford, A. (2012). Anova and ancova: A glm approach. Hoboken, New Jersey: John Wiley & Sons, Inc. [ProQuest](https://ebookcentral.proquest.com/lib/ncent-ebooks/detail.action?docID=1011369).

> Provides an in-depth treatment of ANOVA and ANCOVA techniques from a linear model perspective ANOVA and ANCOVA: A GLM Approach provides a contemporary look at the general linear model (GLM) approach to the analysis of variance (ANOVA) of one- and two-factor psychological experiments. With its organized and comprehensive presentation, the book successfully guides readers through conventional statistical concepts and how to interpret them in GLM terms, treating the main single- and multi-factor designs as they relate to ANOVA and ANCOVA. The book begins with a brief history of the separate development of ANOVA and regression analyses, and then goes on to demonstrate how both analyses are incorporated into the understanding of GLMs. This new edition now explains specific and multiple comparisons of experimental conditions before and after the Omnibus ANOVA, and describes the estimation of effect sizes and power analyses leading to the determination of appropriate sample sizes for experiments to be conducted. Topics that have been expanded upon and added include: Discussion of optimal experimental designs Different approaches to carrying out the simple effect analyses and pairwise comparisons with a focus on related and repeated measure analyses The issue of inflated Type 1 error due to multiple hypotheses testing Worked examples of Shaffer's R test, which accommodates logical relations amongst hypotheses ANOVA and ANCOVA: A GLM Approach, Second Edition is an excellent book for courses on linear modeling at the graduate level. It is also a suitable reference for researchers and practitioners in the fields of psychology and the biomedical and social sciences.

### 1: Introduction to General Linear Models: Regression, Analysis of Variance, and Analysis of Covariance

The first chapter provides a refresher of the regression, ANOVA and ANOCA.  This information was skimmed due to being fairly redundant with existing materials.

One critical difference is the text places strong emphasis on using matrix computations through software, versus scalar calculations.  This approach makes a lot of sense as high dimensional computations are more clearly expressed through this format.

### 2: Traditional and GLM Approaches to Independent Measures Single Factor ANOVA Designs

The next chapter provides a refresher on confidence intervals, sum of square errors, and other metrics for assessing the accuracy of a statistic.

### 3: Comparing Experimental Condition Means, Multiple Hypothesis Testing, Type 1 Error, and a Basic Data Analysis Strategy

There are three basic stages of data analysis:

1. Apply the omnnibus ANOVA and determine the Mean Square Error rate (see: `Sangseok Lee, & Dong Kyu Lee. (2018)`)
2. Interpret the results of the omnibus ONOVA and identify any specific and theoretically relevant comparisons
3. Examine the next level of details and conduct pairwise comparisons

### 4: Measures of Effect Size and Strength of Association, Power, and Sample Size

This chapter appears to largely be redundant from material from [Week 3 Videos](../../Week3_Design/Videos).

### 5: GLM Approaches to Independent Measures Factorial Designs

A factorial design takes into account multiple variables at the same time.  These configurations are quiet common in the real-world.

## Exploring data in R (2018)

Shaughnessy, A., Prener, C., & Hasenmueller, E. (2018). Exploring data in R. [GitHub](https://shaughnessyar.github.io/driftR/articles/ExploringData.html).  [ExploringDataR.pdf](ExploringDataR.pdf).

This tutorial shows how to load data into an R-script, then perform the various calculations discussed in this weeks material.

## How to Select Appropriate Statistical Tests in Scientific Articles (2016)

Trajkovski, V. (2016). How to Select Appropriate Statistical Tests in Scientific Articles. Journal of Special Education & Rehabilitation. 7(3/4), 5–28. [https://doi-org.proxy1.ncu.edu/10.19057/jser.2016.7](https://doi-org.proxy1.ncu.edu/10.19057/jser.2016.7). [SelectStatisticalTests.pdf](SelectStatisticalTests.pdf).

A common challenge in research is choosing the correct statistical test to describe the specific scenario.  When inexperienced authors use the wrong metric it lowers the credibility of the work and can provide inaccuate conclusions.  Several large journals are addressing these issues with dedicated editor of statistics, however, this role is still under represented in the broader publishing world.

### What are parametric versus non-parametric methods

A parametric distribution (e.g., normal distribution) allows the researchers to make certain assumptions about the likelihood of values appearing.  However, many real-life data sets have multiple classes or ranges of values that are more common than others (e.g., W and M shapes).  

When parametric tests are applied to non-parametric data, then the resulting calculations are inaccurate.

![parametric_vs_nonparametric.png](parametric_vs_nonparametric.png)

### What tests are valid for given feature

The given feature type dictates which statistical tests are compatible with its values.  For instance, it would not make sense to take the average of a nominal scale (e.g., categorical value), but determining a frequence ratio does.

| Data Type | Description| Example |
|-----------|-----------|---------|
|Nominal | Categorical| Gender or color|
|Ordinal|Ordered Qualitative| sad, happy, excited|
|Interval| Scaled values| age in years or weight in km|
|Ratio| Combines previous three into one value| $100 versus $1000 dollars|
