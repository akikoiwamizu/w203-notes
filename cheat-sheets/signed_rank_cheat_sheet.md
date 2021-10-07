# Cheat Sheet: Wilcoxon Signed Rank Test

This is a nonparametric test for paired data.  Each unit of observation is represented by a pair of random variables, $(X, Y)$, and the test compares the mean of $X$ against the mean of $Y$.  For example, it can be used to compare grip strength before taking a vitamin against grip strength after taking a vitamin.  Even though this test is nonparametric, it technically requires a metric scale.


Assumptions:

1. Metric scale.
    - In particular, X and Y are both measured on the same metric scale.
2. IID data.
    - In particular, each pair $(X_i,Y_i)$ is drawn from the same distribution, independently of all other pairs.
3. The distribution of the difference $X - Y$ is symmetric around some mean $\mu$
  
Null Hypothesis:

The expectation of $X$ equals the expectation of $Y$.

- In other words, $\mu = 0$.


# Cheat Sheet: Sign Test

This is a nonparametric test for paired data.  Each unit of observation is represented by a pair of random variables, $(X, Y)$.  For example, it can be used to compare scores on a pre-test against scores on a post-test, when the scores should not be treated as metric.  Unlike the Wilcoxon Signed-Rank Test, the Sign Test does not require a metric scale.  However, it generally offers much less power.


Assumptions:

1. Ordinal scale.
    - In particular, X and Y are both measured on the same ordinal scale.
2. IID data.
    - In particular, each pair $(X_i,Y_i)$ is drawn from the same distribution, independently of all other pairs.
  
Null Hypothesis:

The probability of a decreasing pair $(X>Y)$ is the same as the probability of an increasing pair $(X<Y)$.
