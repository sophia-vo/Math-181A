# Higher Moments

The mean and the variance are case of the *moments* of a random variable. Specifically, $E(W)$ is the *first moment about the origin* and $\sigma^2$ is the *second moment about the mean*. $E(W)$ and $\sigma^2$ reflect a random variable's location and dispersion. The skewness of a distribution $\textemdash$ that is, the extent to which it is not summetric around $\mu \textemdash$ can be measured in terms of a *third* moment. The flatness of a pdf can be quantified by the *fourth* moment.

### Definition

Let $W$ be any random variable with pdf $f_W(w). For any positive integer $r$,

&nbsp; **a.** The *r*th *moment of W about the origin*, $\mu_r$, is given by 

$$\mu_r = E(W^r)$$ 

&nbsp; &nbsp; &nbsp; provided $\int_{- \infty}^{\infty} |w|^r \cdot f_W(w)dw < \infty$ (or provided the analogous condition on the *summation* of $|w|^r$ holds, if $W$ is discrete).

&nbsp; **b.** The *r*th *moment of* $W$ *about the mean*, $\mu_r\'$, is given by 

$$\mu_r\' = E\[(W-\mu)^r\]$$ 

&nbsp; &nbsp; &nbsp; provided the finiteness conditions of part 1 hold.

### Theorem

If the $k\text{th}$ moment of a random variable exists, all moments of order less than $k$ exist.


