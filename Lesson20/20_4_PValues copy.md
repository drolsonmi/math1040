<head>
<title>20.4 Calculating P-Values</title>
<script>
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']]
  }
};
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 20.4 Calculating P-Values
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.3.4 p-values (pages 201–203)

## Lesson

In Lesson 20.3, we rejected or failed to reject the null hypothesis by comparing a test statistic to a critical value. A second — and very common — method is to calculate a **p-value**.

#### What is a P-Value?

The **p-value** is the probability of obtaining a sample result at least as extreme as the one observed, *assuming the null hypothesis is true*.

* A **small** p-value means the observed data would be very unlikely under $$H_0$$, so we have strong evidence against it.
* A **large** p-value means the observed data are consistent with $$H_0$$, so we lack evidence to reject it.

#### The Decision Rule

$$\text{If } p\text{-value} \le \alpha, \text{ reject } H_0.$$
$$\text{If } p\text{-value} > \alpha, \text{ fail to reject } H_0.$$

This is equivalent to the critical region approach — the two methods always give the same conclusion.

#### Computing the P-Value

Once you have the test statistic (z or t), the p-value is found from the corresponding distribution:

| Test Type | p-value |
|---|---|
| Right-tailed ($$H_A: \mu > \mu_0$$) | $$P(Z > z)$$ or $$P(T > t)$$ |
| Left-tailed ($$H_A: \mu < \mu_0$$) | $$P(Z < z)$$ or $$P(T < t)$$ |
| Two-tailed ($$H_A: \mu \ne \mu_0$$) | $$2 \cdot P(Z > |z|)$$ or $$2 \cdot P(T > |t|)$$ |

On the TI-84, use `normalcdf` for z-tests and `tcdf` for t-tests.

#### Example

> American mental abilities are often measured by an IQ test. The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

From the previous lesson, we found:
* $$H_0: \mu = 100 \qquad H_A: \mu > 100$$ (right-tailed)
* Test statistic: $$z = 2.656$$

**P-value** (right-tailed):

$$p = P(Z > 2.656) = 1 - P(Z < 2.656) = 1 - 0.9961 = 0.0039$$

On the TI-84: `normalcdf(2.656, 1E99, 0, 1)` gives $$p \approx 0.0040$$.

**Decision:** $$p = 0.0040 \le \alpha = 0.05$$, so we **reject $$H_0$$**.

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the average IQ of Snow College students is higher than the national average.

Notice that this is the same conclusion we reached with the critical region method. The two approaches are always equivalent.

## Practice
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, use the p-value method to test the claim.
    * [After solving on your own, see solution here](Solutions/20_4_Solution1.md)

2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A random sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level using the p-value method.
    * [After solving on your own, see solution here](Solutions/20_4_Solution2.md)

3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. A random sample of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level using the p-value method.
    * [After solving on your own, see solution here](Solutions/20_4_Solution3.md)

## Technology
### TI-83/84
#### P-value from a z-test statistic
* Press `2nd` → `[DISTR]`
* Select `2:normalcdf(`
* **Right-tailed:** `normalcdf(z, 1E99, 0, 1)`
* **Left-tailed:** `normalcdf(-1E99, z, 0, 1)`
* **Two-tailed:** `2 × normalcdf(|z|, 1E99, 0, 1)`

#### P-value from a t-test statistic
* Press `2nd` → `[DISTR]`
* Select `5:tcdf(`
* **Right-tailed:** `tcdf(t, 1E99, df)`
* **Left-tailed:** `tcdf(-1E99, t, df)`
* **Two-tailed:** `2 × tcdf(|t|, 1E99, df)`
