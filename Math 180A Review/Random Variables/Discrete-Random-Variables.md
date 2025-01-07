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

$$p_X(k) = P(| s \in S | X(s) = k |)$$

Note that $p_X(k) = 0$ for any $k$ not in the range of $X$. For notational simplicity, we delete all references to $s$ and $S$ and write $p_X(k) = P(X-k)$.

## Expectation
### Definition

Let $X$ be a discrete random variable with probability function $p_X(k)$. The *expected value of* $X$ is denoted $E(X)$ (or sometimes $\mu$ or $\mu_X$) and is given by 

$$E(X) = \mu = \mu_X = \sum_{\text{all $k$}} k \cdot p_X(k)$$
