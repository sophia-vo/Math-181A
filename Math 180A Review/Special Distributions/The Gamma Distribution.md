# The Gamma Distribution

> Suppose a series of indepedent events are occurring at the constant rate of $\lambda$ per unit time. If the random variable $Y$ denotes the interval between consecutive occurrences, $f_Y(y) = \lambda e^{- \lambda y}, y > 0$. Equivalently, $Y$ can be interpreted as the "waiting time" for the first occurrence. This generalizes the Poisson/exponential relationship, focusing on the interval, or waiting time, required for the $r$th event to occur.

## Theorem
Suppose that Poisson events are occurring at the constant rate of $\lambda$ per unit time. Let the random variable $Y$ denote the waiting time for the $r$th event. Then $Y$ has pdf $f_Y(y)$, where

$$f_Y(y) = \frac{\lambda^r}{(r-1)!} y^{r-1} e^{- \lambda y} , \quad y>0$$

### Definition
For any real number $r>0$, the *gamma function of* $r$ is denoted $\Gamma(r)$, where

$$\Gamma(r) = \int_0^{\infty} y^{r-1}e^{-y}dy$$

> ### Theorem
> Let $\Gamma(r) = \int_0^{\infty} y^{r-1}e^{-y}dy$ for any real number $r>1$. Then
> 
> &nbsp; **a.** $\Gamma(1) = 1$
> 
> &nbsp; **b.** $\Gamma(r) = (r-1) \gamma(r-1)$
> 
> &nbsp; **c.** If $r$ is an integer, then $\Gamma(r) = (r-1)!$

## Definition
Given real numbers $r>0$ and $\lambda > 0$, the random variable $Y$ is said to have the *gamma pdf* with parameters $r$ and $\lambda$ if

$$f_Y(y) = \frac{\lambda^r}{\Gamma(r)}y^{r-1}e^{- \lambda y}, \quad y \geq 0$$

Suppose that $Y$ has a gamma pdf with parameters $r$ and $\lambda$. Then

$$E(Y) = r/ \lambda$$

$$\text{Var}(Y) = r / \lambda^2$$
