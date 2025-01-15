# Estimation

> Any function of a random sample whose objective is to approximate a parameter is called a *statistic*, or an *estimator*. If $\theta$ is the parameter being approximated, its estimator will be denoted $\hat{\theta}$. When an estimator is evaulated (by subsituting the actual measurements recorded), the resulting number is called an *estimate*.

## Estimating Parameters: The Method of Moments (MME)

Suppose that $Y$ is a continuous random variable and that its pdf is a function of $s$ unknown parameters, $\theta_1, \theta_2, \ldots, \theta_s$. The first $s$ moments of $Y$, if they exist, are given by the integrals

$$E(Y^j) = \int_{- \infty}^{\infty} y^j \cdot f_Y(y; \theta_1, \theta_2, \ldots, \theta_s)dy, \quad j=1, 2, \ldots, s$$

In general, each $E(Y_j)$ will be a different function of the $s$ parameters. That is,

$$\begin{align}
E(Y^1) & = g_1(\theta_1, \theta_2, \ldots, \theta_s) \\
E(Y^2) & = g_2(\theta_1, \theta_2, \ldots, \theta_s) \\
& \vdots \\
E(Y^s) & = g_s(\theta_1, \theta_2, \ldots, \theta_s)
\end{align}$$

Corresponding to each *theoretical* moment, $E(Y^j)$, is a *sample* moment, $\frac{1}{n} \sum_{i=1}^n e_i^j$. 

Intuitively, the $j\text{th}$ sample moment is an approximation to the $j\text{th}$ theoretical moment. Setting the two equal *for each* $j$ produces a system of $s$ simultaneous equations, the solutions to which are the desired set of estimates, $\hat{\theta_1}, \hat{\theta_2}, \ldots,$ and $\hat{\theta_s}$.

### Definition
Let $y_1, y_2, \ldots, y_n$ be a random sample from the continuous pdf $f_Y(y; \theta_1, \theta_2, \ldots, \theta_s)$. The *method of moments* estimates (MME), $\hat{\theta_1}, \hat{\theta_2}, \ldots$, and $\hat{\theta_s}$, for the model's unknown parameters are the solutions of the $s$ simultaneous equations

$$E(Y) = \frac{1}{n} \sum_{i=1}^n y_i ; \quad E(Y^2) = \frac{1}{n} \sum_{i=1}^n y_i^2 ; \ldots; E(Y^s) = \frac{1}{n} \sum_{i=1}^n y_i^s$$

If the underlying random variable $X$ is discrete with $p_X(k;\theta_1,\theta_2,\ldots,\theta_s)$, the method of moments estimates are the solutions of the system of equations,

$$E(X^j) = \frac{1}{n} \sum_{i=1}^n k_i^j, \quad j=1, \ldots, s$$

## Estimating Parameters: The Method of Maximum Likelihood (MLE)

> It seems plausible to choose as the estimate for $\theta$ the value of the parameter that maximizes the "likelihood" of the sample. The latter is measured by a *likelihood function*, which is simply the product of the underlying pdf evauated for each of the data points.

### Definition
Let $k_1,k_2, \ldots, k_n$ be a random sample of size $n$ from the discrete pdf $p_X(k; \theta)$, where $\theta$ is an unknown parameter. The *likelihood function*, $L(\theta)$, is the product of the pdf evaluated at the $n$ $k_i\text{'s}$. That is,

$$L(\theta) = \prod_{i=1}^n p_X(k_i;\theta)$$

If $y_1,y_2,\ldots,y_n$ is a random sample of size $n$ from a continuous pdf, $f_Y(y;\theta)$, where $\theta$ is an unknown parameter, the likelihood function is written

$$L(\theta) = \prod_{i=1}^n f_Y(y_i;\theta)$$

### Definition

Let $L(\theta) = \prod_{i=1}^n p_X(k_i;\theta)$ and $L(\theta) = \prod_{i=1}^n f_Y(y_i;\theta)$ be the likelihood functions corresponding to random samples $k_1,k_2,\ldots,k_n$ and $y_1,y_2,\ldots,y_n$ drawn from the discrete pdf $p_X(k;\theta)$ and continuous pdf $f_Y(y;\theta)$, respectively, where $\theta$ is an unknown parameter. In each case, let $\hat{\theta}$ be a value of the parameter such that $L(\hat{\theta}) \geq L(\theta)$ for all possible values of $\theta$. Then $\hat{\theta}$ is called a *maximum likelihood estimate* for $\theta$.
