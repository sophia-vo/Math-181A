# Discrete Random Variables

## Discrete Probability Function
### Definition
Suppose that $S$ is a finite or countably infinite sample space. Let $p$ be a real-valued function defined for each element of $S$ such that

&nbsp; **a.** $0 \leq p(s)$ for each $s \in S$\
&nbsp; **b.** $\sum_{s \in S} p(s) = 1$

Then $p$ is said to be a *discrete probability function*.

> Once $p(s)$ is defined for all $s$, it follows that the probability of any event $A \textemdash$ that is, $P(A) \textemdash$ is the sum of the probabilities of the outcomes comprising $A$:
>
> $$P(A) = \sum_{s \in A} p(s)$$

## Discrete Random Variable
### Definition

A function whose domain is a sample space $S$ and whose values form a finite or countable infinite set of real numbers is called a *discrete random variable*. We denote random variables by uppercase letters, often $X$ or $Y$.

## The Probability Density Function
### Definition

Associated with every discrete random variable $X$ is a *probability density function (or pdf)*, denoted $o_X(k)$, where

$$p_X(k) = P( s \in S | X(s) = k )$$

Note that $p_X(k) = 0$ for any $k$ not in the range of $X$. For notational simplicity, we delete all references to $s$ and $S$ and write $p_X(k) = P(X-k)$.

## Expectation
### Definition

Let $X$ be a discrete random variable with probability function $p_X(k)$. The *expected value of* $X$ is denoted $E(X)$ (or sometimes $\mu$ or $\mu_X$) and is given by 

$$E(X) = \mu = \mu_X = \sum_{\text{all $k$}} k \cdot p_X(k)$$

### Theorem

Suppose $X$ is a discrete random variable with pdf $p_X(k)$. Let $g(X)$ be a function of $X$. Then the expected value of the random variable $g(X)$ is given by

$$E\[g(X)\] = \sum_{\text{all $k$}} g(k) \cdot p_X(k)$$

provided that $\sum_{\text{all }k} |g(k)| p_X(k) < \infty$.

### Corollary

For any random variable $W$, $E(aW+b) = aE(W)+b$, where $a$ and $b$ are constants.

## Variance

> ### An Incorrect Approach
>
> Suppose that $X$ is any discrete random variable. One seemingly reasonable approach would be to average the deviations of $X$ from their mean $\textemdash$ that is, calculate the expected value of $X-\mu$. This strategy will not work because the negative deviations will exactly cancle the positive deivations, making the numerical value of such an average always zero, regardless of the amount of spread present in $p_X(k)$:
>
> $$E(X-\mu) = E(X) - \mu = \mu - \mu = 0$$

### Definition
The *variance* of a random variable is the expected value of its squared deviations from $\mu$. If $X$ is discrete, with pdf $p_X(k)$, 

$$\text{Var}(X) = \sigma^2 = E\[(X-\mu)^2\] = \sum_{\text{all $k$}} (k- \mu)^2 \cdot p_X(k)$$

> ### Comment
> The units for the variance are the square of the units for the random variable. Where unit compatibility is important, dispersion is measured by the *standard deviation*, which is defined to be the square root of the variance. That is,
>
> $$\sigma = \text{standard deviation} = \sqrt{\sum_{\text{all $k$}} (k- \mu)^2 \cdot p_X(k)}$$

> [!IMPORTANT]
> The two theorems below apply to both discrete and continuous random variables.

### Theorem
Let $W$ be any random variable, discrete or continuous, having mean $\mu$ and for which $E(W^2)$ is finite. Then

$$\text{Var}(W) = \sigma^2 = E(W^2) - \mu^2$$

### Theorem
Let $W$ be any random variable having mean $\mu$ and where $E(W^2)$ is finite. Then $\text{Var}(aW + b) = a^2 \text{Var}(W)$.


