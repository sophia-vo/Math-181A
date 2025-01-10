# Properties of Frequently Used pdfs

## Discrete models

### Binomial: $X \sim Binom(n,p), \quad X \in$ { $0,1,2, \ldots, n$ }

> $X$ is the number of successful trials out of the $n$ total trials. Each trial has success probability $p$.

Given: $n$ independent trials, each having probability $p$ of success

$$\begin{align}
\text{Let } X & = \text{number of successes} \\
p_X(k) & = P(k \text{ successes occur in } n \text{ trials}) \\
& = {n \choose k} p^k (1-p)^{n-k}, \quad k=0,1,\ldots,n \\
\\
E(X) & = np \\
\text{Var}(X) & = np(1-p)
\end{align}$$

### Geometric: $X \sim Geom(p), \quad X \in$ { $1,2,3, \ldots$ }

> $X$ is the number of trials needed to get the first success including tne success), Each trial has success probability $p$.

Given: $n$ independent trials, each having probability $p$ of success

$$\begin{align}
\text{Let } X & = \text{trial where first success occurs} \\
p_X(k) & = P(\text{First success occurs on } k \text{th trial}) \\
& = (1-p)^{k-1}p, \quad k=1, 2, \ldots \\
\\
E(X) & = \frac{1}{p} \\
\text{Var}(X) & = \frac{(1-p)}{p^2}
\end{align}$$

### Negative Binomial: $X \sim NegBinom(r,p), \quad X \in$ { $r,r+1,r+2, \ldots$ }

> $X$ is the number of trials needed to get the $r^{th}$ success (so $r$ total successes). Each trial has success probability $p$.

Given: $n$ independent trials, each having probability $p$ of success

$$\begin{align}
\text{Let } X & = \text{trial where} r \text{th  success occurs} \\
p_X(k) & = P(r\text{th success occurs on } k \text{th trial}) \\
& = {{k-1} \choose {r-1}} p^r (1-p)^{k-r}, \quad k=r, r+1, r+2, \ldots \\
\\
E(X) & = \frac{r}{p} \\
\text{Var}(X) & = \frac{r(1-p)}{p^2}
\end{align}$$

> When $r=1$, this collapses to the Geometric distribution. $NegBinom(r,p)$ is the sum of $r$ $Geom(p)$ RVs.

### Poisson $X \sim Poisson(\lambda), \quad X \in$ { $0,1,2, \ldots$ }

> $X$ is the number of times an event occurs in a given time when its average rate of occurrence in that time is $\lambda$.

Given: a series of events occurring independently at a constant rate of $\lambda$ per unit time (or volume or space)

$$\begin{align}
\text{Let } X & = \text{number of occurrences in unit time (or volume or space)} \\
p_X(K) & = P(k \text{ events occur in unit time (or volume or space)}) \\
& = \frac{e^{- \lambda} \cdot \lambda^k}{k!}, \quad k = 0,1,2,\ldots \\
\\
E(X) & = \text{Var}(X) = \lambda 
\end{align}$$

> The units on $\lambda$ (rate) are:
>
> $$\lambda = \frac{\text{number of events}}{\text{time spa for measurement}}$$

## Continuous

### Uniform: $X \sim Unif(a,b)$

> $X$ is an output in a finite range for which all outcomes in the range are equally likely.

$$\begin{align}
f(x) & =
\begin{cases}
\frac{1}{b-a}, & a \leq x \leq b \\
0, & \text{else}
\end{cases} \\
\\
E(X) & = \frac{a+b}{2} \\
\text{Var}(X) & = \frac{(b-a)^2}{12}
\end{align}$$

> Recall, all density functions satisfy:  
> &nbsp; **1)** $f(x) \geq 0$ for all values of $x$
> &nbsp; **2)** $\int_{- \infty}^{\infty} f(x) dx = 1$

### Exponential $X \sim Exp(\lambda)$

> $X$ represents how long we must wait for an event to occur when we know how often it occurs on average $(\lambda)$.

$$\begin{align}
f_X(x) & = \lambda e^{- \lambda x}, \quad x \geq 0 \\
\text{alternatively, } f(x) & =
\begin{cases}
\lambda e^{- \lambda x}, & x \geq 0 \\
0, & \text{else}
\end{cases} \\
\\
E(X) & = \frac{1}{\lambda} \\
\text{Var}(X) & = \frac{1}{\lambda^2}
\end{align}$$


### Gamma: $X \sim Gamma(r, \lambda)$

> $X$ represents the time required to see $r$ instances of an event that occurs with average rate $\lambda$.  
> If $r \in \mathbb{N}$, then $Gamma(r,\lambda) = \sum_1^r Exp(\lambda)$.

$$\begin{align}
f_X(x) & = \left(\frac{\lambda^r}{\gamma(r)}\right)x^{r-1}e^{- \lambda x}, \quad x>0, r>0, \lambda>0 \\
\\
E(X) & = \frac{r}{\lambda} \\
\text{Var}(X) & = \frac{r}{\lambda^2}
\end{align}$$

### Normal: $X \sim N(\mu, \sigma^2)$

> $X$ represents a real world phenomenum that follows a bell-curve distribution.

$$\begin{align}
f_X(x) & = \frac{1}{\sqrt{2 \pi} \sigma} e^{- \frac{1}{2} \left(\frac{x-\mu}{\sigma}\right)^2}, \quad - \infty < x < \infty \\
\\
E(X) & = \mu \\
\text{Var}(X) & = \sigma^2
\end{align}$$


