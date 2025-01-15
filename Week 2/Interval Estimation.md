# Interval Estimation

> The usual way to quantify the amount of uncertainty in an estimator is to con-struct a *confidence interval*. In principle, confidence intervals are ranges of numbers that have a high probability of “containing” the unknown parameter as an interior point. By looking at the *width* of a confidence interval, we can get a good sense of the estimator’s precision.

## Confidence Intervals for the Binomial Parameter $p$
### Theorem
Let $k$ be the number of successes in $n$ indepedent trials, where $n$ is large and $p = P(\text{success})$ is unknown. An approximate $100(1-\alpha)%$ confidence interval for $p$ is the set of numbers

$$\frac{k}{n} - z_{\alpha/2} \sqrt{\frac{(k/n)(1-k/n)}{n}}, \frac{k}{n} + z_{\alpha/2} \sqrt{\frac{(k/n)(1-k/n)}{n}}$$

### Definition
The *margin of error* associated with an estimate $\frac{k}{n}$, (for a 95% confidence interval), where $k$ is the number of successes in $n$ indepdent trials, is $100d\text{%}$, where $d = \frac{1.96}{2\sqrt{n}}$.

In general, for a $100(1-\alpha\text{%}$ confidence interval, the margin of error is $d = \frac{z_{\alpha/2}}{2\sqrt{n}}$, where $z_{\alpha/2}$ is the value for which $P(Z \geq z_{\alpha/2}) = \alpha/2$.

The margin of error is often expressed as a percentage, in which case it would be $100d\text{%}$.

### Theorem

let $\frac{X}{n}$ be the estimator for the parameter $p$ in a binomial distribution. In order for $\frac{X}{n}$ to have at least a $100(1-\alpha)\text{%}$ probability of being within a distance $d$ of $p$, the sample size should be no smaller than

$$n = \frac{Z_{\alpha/2}^2}{4d^2}$$
