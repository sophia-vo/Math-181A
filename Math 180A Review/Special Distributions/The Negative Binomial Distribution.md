# The Negative Binomial Distribution

The negative binomial distribution is a generalization of the geometric distribution, representing the waiting time for the $r$th (instead of the first) success in a series of independent trials, where each trial has a probability of $p$ of ending in success. 

> There are $r-1$ successes and $k-1-(r-1)$ failures, with one success, the $r$th success. There are $k$ indepedent trials.

Let the random variable $X$ denote the trial at which the $r$th success occurs. Then

$$\begin{align}
p_X(k) = P(X=k) & = P(r \text{th success occurs on } k \text{th trial}) \\
& = P(r-1 \text{ successes occur in first } k-1 \text{ trials and success occurs on } k \text{th trial}) \\
& = P(r-1 \text{successes occur in first } k-1 \text{ truaks}) \cdot P(\text{Success occurs on } k \text{th trial}) \\
& = {{k-1} \choose {r-1}} p^{r-1} (1-p^{k-1-(r-1)}) \cdot p \\
& = {{k-1} \choose {r-1}} p^r (1-p)^{k-r}, \quad k=r, r+1, \ldots
\end{align}$$

Any random variable whose pdf has the form given in the equation above has the *negative binomial distribution* (with parameters $r$ and $p$).

## Theorem

Let $X$ have a negative binomial distribution with $p_X(k) = {{k-1} \choose {r-1}} p^r (1-p)^{k-r}, \quad k=r, r+1,  \ldots$. Then

$$E{X} = \frac{r}{p}$$

$$\text{Var}(X) = \frac{r(1-p)}{p^2}$$
