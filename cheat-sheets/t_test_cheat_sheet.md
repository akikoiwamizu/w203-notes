# Cheat Sheet: Two-Sample t-Test

This is a parametric test for unpaired data.  It is used to compare the mean of one random variable $X$ against the mean of another random variable $Y$.  For example, you can use a two-sample t-test to compare wait times for domestic and international callers.

Assumptions:

1. Metric scale.  
    - In particular, the t-test is not valid for variables which only have an ordinal structure.
2. IID data.
3. No major deviations from normality, considering the sample size.
    - In particular, the t-test is invalid for highly skewed distributions when sample size is larger than 30.  It may also be invalid for very highly skewed distributions at higher sample sizes.
  
Null Hypothesis:

The expectation of $X$ equals the expectation of $Y$.
  
Notes:

You may hear that the t-test requires an assumption of equal variances for the two groups.  This was true for the original version of the t-test.  However, Welch's version of the t-test (the default in most statistical software) does not require equal variances.