# Readings

## Statistical conclusion validity (2012)

> This resource explains the concept of statistical conclusion validity and provides suggestions for increasing statistical conclusion validity.

García-Pérez, M. A. (2012). Statistical conclusion validity: Some common threats and simple remedies. Frontiers in Psychology, 3. [https://doi.org/10.3389/fpsyg.2012.00325](https://doi.org/10.3389/fpsyg.2012.00325). [StatisticalConclusion.pdf](StatisticalConclusion.pdf).

### Are researchings correctly publishing statistically conclusions

A reoccuring challenge with statistical applications in research, is that the modeling is wrong.  When papers use erroneous calculations or do not correctly meet the threshold of the stated confidence interval, it creates invalid generalizations.  These results compound into the body of knowledge, with additional efforts building until eventually being proven wrong.

> More recently, Bakker and Wicherts (2011) conducted a thorough analysis of psychological papers and estimated that roughly 50% of published papers contain reporting errors, although they only checked whether the reported p value was correct and not whether the statistical test used was appropriate. A similar analysis carried out by Nieuwenhuis et al. (2011) revealed that 50% of the papers reporting the results of a comparison of two experimental effects in top neuroscience journals had used an incorrect statistical procedure. And Bland and Altman (2011) reported further data on the prevalence of incorrect statistical analyses of a similar nature.

### What is the influence of the sampling process

Research with `fixed sampling` choose the number of data points, collects the data, then performs the analysis.  In contrast `sequential sampling` uses an iterative model of collect, analyze, optionally repeat.

There are strengths and weaknesses to both strategies. For instance, fixed runs the risk of wasting significant resources before reaching a dead end.  However, sequential might give an inaccurate picture due to incomplete coverage.

> Frick (1998) proposed that repeated statistical testing be conducted under the so-called COAST (composite open adaptive sequential test) rule: If the test yields p < 0.01, stop collecting data and reject the null; if it yields p > 0.36, stop also and do not reject the null; otherwise, collect more data and re-test. The low criterion at 0.01 and the high criterion at 0.36 were selected through simulations so as to ensure a final Type-I error rate of 0.05 for paired-samples t tests.

### How can regression analysis help

Researchers can avoid the "damned if you do, damned if you dont" paradox of fixed versus sequential sampling by feeding partial datasets into logistic regression and correlation functions.  These strategies can tease-out structure and provide insights into the underlying structure and determine if appropriate coverage exists for each cluster.

### What is the key final take-aways

> Most breaches of SCV arise from a poor understanding of statistical procedures and the resultant inadequate usage. These problems can be easily corrected, as illustrated in this paper, but the problems will not have arisen if researchers had had a better statistical training in the first place. [...]  One way to eradicate the problem is by improving statistical education at undergraduate and graduate levels, perhaps not just focusing on giving formal training on a number of methods but by providing students with the necessary foundations that will subsequently allow them to understand and apply methods for which they received no explicit formal training.

## Designing and reporting experiments in psychology (2008)

> Chapters 9-13 cover design of experiments, including concepts such as internal and external validity.  Chapters 13 covers more advanced designs.  Chapters 10-12 are most critical. Please note that while the textbook covers concepts within a psychology framework, the concepts apply to all fields.

Harris, P. (2008). Designing and reporting experiments in psychology. New York, NY: McGraw-Hill Education. [ProQuest eBook](https://ebookcentral.proquest.com/lib/ncent-ebooks/detail.action?docID=345135). [DesignReportExperiments_Section2.pdf](DesignReportExperiments_Section2.pdf).

## Threats to the Validity of Research (1993)

> This article provides an excellent overview of threats to validity in research design, which includes the four major types of validity (internal, external, statistical conclusion, and construct validity).

Parker, R. M. (1993). Threats to the Validity of Research. Rehabilitation Counseling Bulletin, 36(3), 130–138. [Direct Link](https://search-ebscohost-com.proxy1.ncu.edu/login.aspx?direct=true&db=eric&AN=EJ458938&site=eds-live).  [ThreatsToValidity.pdf](ThreatsToValidity.pdf).

> It is a widely accepted truism that all published research is flawed to some extent. Because the research enterprise is fraught with many pitfalls, researchers must become well versed in recognizing and, when possible, avoiding design shortcomings.

### What are internal/external threats to validation

These classes of issues can originate from internal and external sources.  For instance, determining causality could be skewed by poor selections by the researcher (`internal threats`) or volunteers sneaking into the study from the same group (`external threats`).  In either situtation the results are the same and e.g., `selection bias` creates an inaccurate representation.

- History of extraneous events
- Maturity of data set
- Testing processes
- Instrumentation and accuracy of measurements
- Statistical regression and inaccurate categorization
- Selection bias
- Mortality and partial data
- Interactions with selection and data intra dependencies
- Ambiguity of cause effort (A -> B or B -> A)

### What are threats to statistical conclusion validity

- Low statistical power (e.g., too small of sample size)
- Fishing and error rates (e.g., run all permutations until something happens to align)
- Low reliability of measures
- Random irrelevancies and other sources of noise
- Heterogeneity of variables (e.g., too many uncontrolled parameters)

### What are threats to construct validity

- Inadequate preoperational test construction
- Mono-operation and insufficient cross checks
- Mono-method and insufficient inclusion of alternatives (e.g., what is the full taxonomy)
- Changing control policies mid-experiment
- Control group seeks external influences
- Not following the agreed upon control procedures
- Information disclosure of control versus experiment participants
- Resentfulness of participants or creating incentives to lie and cheat
- Evaluation apprehension due to concerns of confidentiality
- Experimenter expectations influencing outcome data
- Nesting independent variables too many levels
