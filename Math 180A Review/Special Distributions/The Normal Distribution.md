# The Normal Distribution

> Another function developed for the purpose of approximating binomial probabilities when $n$ is large is
>
> $$P\left\[ a \leq \frac{X - n\left(\frac{1}{2}\right)}{\sqrt{n\left(\frac{1}{2}\right)\left(\frac{1}{2}\right)}} \leq b \right \] = \frac{1}{\sqrt{2\pi}} \int_a^b e^{z^2 / 2} dz$$
>
> where $X$ is a binomial random variable for which $n$ is large and $p = 1/2$.

### Theorem
(DeMoivre-Laplace) Let $X$ be a binomial random variable defined on $n$ independent trials for which $p=P(\text{success})$. For any numbers $a$ and $b$,

$$\lim_{n \to \infty} P \left \[ a \leq \frac{X - np}{\sqrt{np(1-p)}} \leq b \right \] = \frac{1}{\sqrt{2n}} \int_a^b e^{-z^2/2} dz$$

> ### Comment
> The function $f_Z(z) = \frac{1}{\sqrt{2\pi}} e^{-z^2/2}$ is referred to as the *standard normal* (or *Gaussian*) *curve*. By convention, any random variable whose probabilistic behavior is described by a standard normal curve is denoted by $Z$ (rather than $X, Y,$ or $W$). Since $M_Z(t) = e^{t^2/2}$, it follows that $E(Z) = 0$ and $\text{Var}(Z) = 1$.

## Definition
A random variable $Y$ is said to be normally distributed with mean $\mu$ and variance $\sigma^2$ if

$$f_Y(y) = \frac{1}{\sqrt{2\pi\sigma}}e^{-\frac{1}{2}\left(\frac{y-\mu}{\sigma}\right)^2}, \quad - \infty < y < \infty$$

The symbol $Y ~ N(\mu, \sigma^2)$ will sometimes be used to denote the fact that $Y$ has a normal distribution with mean $\mu$ and variance $\sigma^2$.

### Theorem
Let $Y_1$ be a normally distributed random variable with mean $\mu_1$ and variance $\sigma_1^2$, and let $Y_2$ be a normally distributed random variable with mean $\mu_2$ and variance $\sigma_2^2$. Define $Y = Y_1 + Y_2$. If $Y_1$ and $Y_2$ are independent, $Y$ is normally distributed with mean $\mu_1 + \mu_2$ and variance $\sigma_1^2 + \sigma_2^2$.

### Corollary
Let $Y_1, Y_2, \cdots, Y_n$ be a random sample of size $n$ from a normal distribution with mean $\mu$ and variance $\sigma^2$. Then the sample mean, $\bar{Y} = \frac{1}{n} \sum_{i=1}^n Y_i$, is also normally distributed with mean $\mu$ but with variance equal to $\sigma^2 / n$ (which implies that $\frac{\bar{Y}-\mu}{\sigma / \sqrt{n}}$ is a standard normal random variable, $Z$).

### Corollary
Let $Y_1, Y_2, \cdots, Y_n$ be any set of independent normal random variables with means $\mu_1, \mu_2, \cdots, \mu_n$ and variances $\sigma_1^2, \sigma_2^2, \cdots, \sigma_n^2$, respectively. Let $a_1, a_2, \cdots, a_n$ be any set of constants. Then $Y = a_1 Y_1 + a_2 Y_2 + \ldots + a_n Y_n$ is normally distributed with mean $\mu = \sum -{i=1}^n a_i u_i$ and variance $\sigma^2 = \sum_{i=1}^n a_i^2 o_i^2$.
