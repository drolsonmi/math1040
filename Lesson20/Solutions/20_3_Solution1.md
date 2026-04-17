<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, use the critical region method to test the claim.

## Solution
From the problem we get the following information:
* Null value: $$\mu_0 = 4$$
* Sample size: $$n = 35$$
* Sample mean: $$\bar{x} = 4.6$$
* Sample standard deviation: $$s = 1.2$$
* Significance level: $$\alpha = 0.05$$

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes** (stated in the problem)
* Is the sample large enough? **Yes** ($$n = 35 \ge 30$$)

The Central Limit Theorem holds.

**Step 2 — State the hypotheses**

The wait time is claimed to be no more than 4 minutes; the advocacy group believes it is **longer**.

$$H_0: \mu = 4 \qquad\qquad H_A: \mu > 4 \quad \text{(right-tailed)}$$

**Step 3 — Find the critical value**

For a right-tailed test with $$\alpha = 0.05$$ and $$DF = n - 1 = 34$$ degrees of freedom, the critical t-value is:

$$t_c = 1.691$$

**Step 4 — Compute the test statistic**

Since we only have a sample standard deviation, we use the t-test:

$$t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}} = \frac{4.6 - 4}{1.2/\sqrt{35}} = \frac{0.6}{0.2028} = 2.958$$

**Step 5 — Make a decision**

$$t = 2.958 > t_c = 1.691$$

The test statistic falls in the critical region, so we **reject $$H_0$$**.

**Conclusion:** There is sufficient evidence at the 5% significance level to support the claim that the average wait time is more than 4 minutes.

[Return back to Lesson 20.3](../20_3_CriticalRegions.md#practice)
