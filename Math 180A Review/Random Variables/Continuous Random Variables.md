# Continuous Random Variables
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

## Variance
### Definition
The *variance* of a random variable is the expected value of its squared deviations from $\mu$. If $Y$ is continuous, with pdf $f_Y(y)$, 

$$\text{Var}(Y) = \sigma^2 = E\[(Y-\mu)^2\] = \int_{- \infty}^{\infty} (y-\mu)^2 \cdot f_Y(y)dy$$

The *standard deviation* is 

$$\sigma = \text{standard deviation} = \sqrt{\int_{- \infty}^{\infty} (y-\mu)^2 \cdot f_Y(y)dy}$$

> [!IMPORTANT]
> Additional theorems can be found in the *Discrete Random Variable* section.
