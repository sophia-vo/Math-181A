# The Geometric Distribution

Consider a series of independent trials, each having one of two possible outcomes, success or failure. Let $p = P(\text{Trial ends in success})$. Define the random variable $X$ to be the trial *at which the first success occurs*. 

$$\begin{align}
p_X(k) & = P(X=k) = P(\text{First success occurs on } k \text{ trial}) \\
& = P(\text{First } k-1 \text{ trials end in failure and $k$th trial ends in success}) \\
& = P(\text{First } k-1 \text{ trials end in failure}) \cdot P(k \text{th trial ends in success}) \\
& = (1-p)^{k-1} p, \quad k=1, 2, \ldots
\end{align}$$

> The probability model above is a *geometric distribution* with parameter $p$. There are $k-1$ failures and one success, with $k$ independent trials total.

> ### Comment
> The function $p_X(k) = (1-p)^{k-1}p$, $k = 1, 2, \cdots$ qualifies as a discrete pdf because
>
> **(1)** $p_X(k) \geq 0$ for all $k$ and
> 
> **(2)** $\sum_{\text{all } k } p_X(k)=1$

### Theorem
Let $X$ have a geometric distribution with $p_X(k) = (1-p)^{k-1}p, k=1, 2, \ldots$. Then

$$E(X) = \frac{1}{p}$$

$$\text{Var}(X) = \frac{1-p}(p^2)$$
