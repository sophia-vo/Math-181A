# Continuous Random Variable
### Definition
A probability function $P$ on a set of real numbers $S$ is called *continuous* if there exists a function $f(t)$ such that for any closed interval $\[a, b\] \in S, P(\[a, b\]) =  \int_a^b f(t) dt$. The fucntion $f(t)$ must have the following properties:

&nbsp; **a.** $f(t) \geq 0$ for all $t$.\
&nbsp; **b.** $\int_{- \infty}^\infty f(t)dt = 1$.

Then the probabiltiy $P(A) = \int_A f(t)dt$ for any set $A$ where the integral is defined.

## Continuous Probability Density Functions
### Definition
Let $Y$ be a function from the sample space $S$ to the real numbers. The function $Y$ is called a *continuous random variable* if there exists a function $f_Y(y)$ such that for any real numbers $a$ and $b$ with $a < b$

$$P(a \leq Y \leq b) = \int_a^b f_Y(y)dy$$

## Expectation
### Definition

Let $Y$ be a continuous random variable with pdf $f_Y(y)$,

$$E(Y) = \mu = \mu_Y= \int_{- \infty}^{\infty} y \cdot f_Y(y)dy$$
