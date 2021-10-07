# Cheat Sheet: Wilcoxon Rank Sum Test

This is a nonparametric test for unpaired data.  It is used to compare one random variable $X$ against another random variable $Y$.  The test has several names: Wilcoxon Rank Sum, Mann–Whitney U test, Wilcoxon–Mann–Whitney test.  You will find this test presented in two different versions.  We consider the hypothesis of comparisons version, which is more general, to be the most important.

## Hypothesis of Means Version:


Assumptions:

1. Metric scale.  
2. IID data.
    - Each $X_i$ is drawn from the same distribution, each $Y_i$ is drawn from the same distribution, and all $X_i$ and $Y_i$ are mutually independent.
3. The distribution of $X$ is the same as the distribution of $Y - \Delta$ for some constant $\Delta \in \mathbb{R}$.
    - This means that the distributions have the same shape, just translated from each other.
  
Null Hypothesis:

The expectation of $X$ equals the expectation of $Y$.

- In other words, $\Delta = 0$.
  
## Hypothesis of Comparisons Version:
  
Assumptions:

1. Ordinal  scale.  
2. IID data.
    - Each $X_i$ is drawn from the same distribution, each $Y_i$ is drawn from the same distribution, and all $X_i$ and $Y_i$ are mutually independent.
  
Null Hypothesis:

The probability that a draw from $X$ ranks higher than a draw from $Y$ is the same as the probability that a draw from $Y$ ranks higher than a draw from $X$.

- $P(X>Y) = P(X<Y)$