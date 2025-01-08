# Properties of Frequently Used pdfs

## Discrete models

### Binomial
Given: $n$ independent trials, each having probability $p$ of success

$$\begin{align}
\text{Let } X & = \text{number of successes} \\
p_X(k) & = P(k \text{ successes occur in } n \text{trials}) \\
& = {n \choose k} p^k (1-p)^{n-k}, \quad k=0,1,\ldots,n \\
E(X) & = np \\
\text{Var}(X) & = np(1-p)
\end{align}$$

### Geometric
Given: $n$ independent trials, each having probability $p$ of success

$$\begin{align}
\text{Let } X & = \text{trial where first success occurs} \\
p_X(k) & = P(\text{First success occurs on } k \text{th trial}) \\
& = (1-p)^{k-1}p, \quad k=1, 2, \ldots \\
E(X) & = 1/p \\
\text{Var}(X) & = (1-p)/p^2
\end{align}$$

### Negative Binomial
Given: $n$ independent trials, each having probability $p$ of success

$$\begin{align}
\text{Let } X & = \text{trial where} r \text{th  success occurs} \\
p_X(k) & = P(r\text{th success occurs on } k \text{th trial}) \\
& = {{k-1} \choose {r-1}} p^r (1-p)^{k-r}, \quad k=r, r+1, r+2, \ldots \\
E(X) & = r/p \\
\text{Var}(X) & = \[r(1-p)\]/p^2
\end{align}$$

### Poisson
Given: a series of events occurring independently at a constant rate of $\lambda$ per unit time (or volume or space)

$$\begin{align}
\text{Let } X & = \text{number of occurrences in unit time (or volume or space)} \\
p_X(K) & = P(k \text{ events occur in unit time (or volume or space)}) \\
& = e^{- \lambda} \lambda^k / k!, \quad 0,1,2,\ldots \\
E(X) & = \lambda \\
\text{Var}(X) & = \lambda 
\end{align}$$

## Continuous

### Exponential

$$\begin{align}
f_Y(y) & = \lambda e^{- \lambda y}, \quad y>0 \\
E(Y) & = 1/\lambda \\
\text{Var}(Y) & = 1/ \lambda^2 
\end{align}$$

### Gamma

$$\begin{align}
f_Y(y) & = (\lambda^r / \gamma(r))y^{r-1}e^{- \lambda y}, \quad y>0 \\
E(Y) & = r/ \lambda \\
\text{Var}(Y) & = r/ \lambda^2
\end{align}$$

### Normal

$$\begin{align}
f_Y(y) & = \frac{1}{\sqrt{2 \pi} \sigma} e^{- \frac{1}{2} \left(\frac{y-\mu}{\sigma}\right)^2}, \quad - \infty < y < \infty \\
E(Y) & = \mu \\
\text{Var}(Y) & = \sigma^2
\end{align}$$


