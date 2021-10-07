# Cheat Sheet: Paired t-Test

This is a parametric test for paired data.  Each unit of observation is represented by a pair of random variables, $(X, Y)$, and the test compares the mean of $X$ against the mean of $Y$.  For example, a paired t-test can be used to compare the number of business travelers against the number of leisure travelers for a sample of airlines.

When $X$ and $Y$ are positively correlated, the paired t-test will tend to have more power than an unpaired t-test.


Assumptions:

1. Metric scale.  
    - In particular, the t-test is not valid for variables which only have an ordinal structure.
2. IID data.
    - In particular, each pair of measurements $(X_i, Y_i)$ is drawn from the same distribution, independently of all other pairs.
3. The distribution of the difference between measurements has no major deviations from normality, considering the sample size.
    - In particular, the t-test is invalid for highly skewed distributions when sample size is larger than 30.  It may also be invalid for very highly skewed distributions at higher sample sizes.
  
  
Null Hypothesis:

The expectation of $X-Y$ is zero.