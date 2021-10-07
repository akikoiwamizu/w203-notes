# Cheat Sheet: t-Based Confidence Interval

This is a way to indicate an interval of "plausible" values for a parameter.

Assumptions:

1. Metric scale.  
    - In particular, a confidence interval is not valid for variables which only have an ordinal structure.
2. IID data.
3. No major deviations from normality, considering the sample size.
    - In particular, the t-based confidence interval is invalid for highly skewed distributions when sample size is larger than 30.  It may also be invalid for very highly skewed distributions at lower sample sizes.
  

Note: It is NOT correct to say that there is a 95% chance that a mean is inside a confidence interval.  This is a misapplication of Bayesian logic.  What is correct is that 95% of confidence intervals constructed according to a valid procedure will include the true mean.