# Binomial Probability Distribution

Situations involving a series of independent and identical trials. Each trial can only have one of two possible outcomes.

Consider a series of $n$ independent trials, each resulting in one of two possible outcomes, "success" or "failure."  

Let $p = P$ (success occurs at any given trial) and assume that $p$ remains constant from trial to trial.  Then

$$P(\text{$k$ successes}) = {n \choose k} p^k (1-p)^{n-k}, \quad k = 0, 1, \cdots, n$$

Let the random variable $X$ denote the number of successes in $n$ independent trials, then  

$$P(X=k) = p_X (k) = {n \choose k} p^k (1-p)^{n-k}, \quad k = 0, 1, \cdots , n$$

## Expectation Proof

> Suppose $X$ is a binomial random variable with parameters $n$ and $p$. Then $E(X) = np$.

$E(X)$ for a binomial random variable is the sum

$$\begin{align}
E(X) = \sum_{k=0}^n k \cdot p_X(k) & = \sum_{k=0}^n k {n \choose k} p^k (1-p)^{n-k} \\
& = \sum_{k=0}^n \frac{k \cdot n!}{k! (n-k)!} p^k (1-p)^{n-k} \\
& = \sum_{k=1}^n \frac{n!}{(k-1)!(n-k)!} p^k (1-p)^{n-k}
\end{align}$$

Factoring out $np$:

$$\begin{align} 
E(X) & = np \sum_{k=1}^n \frac{(n-1)!}{(k-1)!(n-k)!}p^{k-1}(1-p)^{n-k} \\
& = np \sum_{k=1}^n {{n-1} \choose {k-1}} p^{k-1} (1-p)^{n-k}
\end{align}$$

Let $j=k-1$. It follows that

$$E(X) = np \sum_{j=0}^{n-1} {{n-1} \choose j} p^j (1-p)^{n-j-1}$$

Letting $m=n-1$ gives

$$E(X) = np \sum_{j=0}^m {m \choose j} p^j (1-p)^{m-j}$$

Since the value of the sum $\sum_{j=0}^m {m \choose j} p^j (1-p)^{m-j}$ is $1$,

$$E(X) = np$$
