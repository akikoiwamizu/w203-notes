# Cheat Sheet: Sign Test

This is a nonparametric test for paired data.  Each unit of observation is represented by a pair of random variables, $(X, Y)$.  For example, it can be used to compare scores on a pre-test against scores on a post-test, when the scores should not be treated as metric.  Unlike the Wilcoxon Signed-Rank Test, the Sign Test does not require a metric scale.  However, it generally offers much less power.


Assumptions:

1. Ordinal scale.
    - In particular, X and Y are both measured on the same ordinal scale.
2. IID data.
    - In particular, each pair $(X_i,Y_i)$ is drawn from the same distribution, independently of all other pairs.
  
Null Hypothesis:

The probability of a decreasing pair $(X>Y)$ is the same as the probability of an increasing pair $(X<Y)$.
