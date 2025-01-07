# The Poisson Distribution

> The limit for $p_X(k) = {n \choose k} p^k (1-p)^{n-k}$ holds when $n$ approaches $\infty$, $p$ approaches $0$, and $np$ remains constant. In practice, Poisson's limit is used to approximate hard-to-calculate binomial probabilities where the values of $n$ and $p$ reflect the conditions of the limit $\textemdash$ that is, when $n$ is large and $p$ is small.

## The Poisson Limit

Suppose $X$ is a binomial random variable, where

$$P(X=k) = p_X(k) = {n \choose k} p^k (1-p)^{n-k}, \quad k = 0, 1, \cdots , n$$

If $n \to \infty$ and $p \to 0$ in such a way that $\lambda = np$ remains constant, then

$$
\lim_{\substack{n \to \infty \\ 
p \to 0 \\ 
np = \text{const.}}} P(X=k) = 
\lim_{\substack{n \to \infty \\ 
p \to 0 \\ 
np = \text{const.}}} 
{n \choose k} p^k (1-p)^{n-k} = \frac{e^{-np} (np)^k}{k!} = \frac{e^{- \lambda} \lambda^k}{k!}
$$

## The Poisson Distribution

The random variable $X$ is said to have a Poisson distribution if

$$p_X(k) = P(X=k)= \frac{e^{- \lambda} \lambda^k}{k!}, \quad k=0, 1, 2, \cdots$$

where $\lambda$ is a positive constant. For any Poisson random variable,

$$E(X) = \lambda$$

$$\text{Var}(X) = \lambda$$

Poisson data invariability refer to the numbers of times a certain event occurs during each of a series of "units" (often *time* or *space*).

### Theorem

Suppose a series of events satisfying the Poisson model are occurring at the rate of $\lambda$ per unit time. Let the random variable $Y$ denote the interval between consecutive events. Then $Y$ has the exponential distribution

$$f_Y(y) = \lambda e^{- \lambda y}, \quad y > 0$$
