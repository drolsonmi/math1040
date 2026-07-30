<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. Conduct a full hypothesis test at the 5% significance level.

## Solution
From the problem we get the following information:
* Null value: $\mu_0 = 4$
* Sample size: $n = 35$, $DF = 34$
* Sample mean: $\bar{x} = 4.6$
* Sample standard deviation: $s = 1.2$
* Significance level: $\alpha = 0.05$

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes** (stated in the problem)
* Is $n \ge 30$? **Yes** ($n = 35$)

The CLT holds.

**Step 2 — State the Hypotheses**

The advocacy group believes the wait time is **longer** than 4 minutes.

$$H_0: \mu = 4 \qquad\qquad H_A: \mu > 4 \quad \text{(right-tailed)}$$

**Step 3 — Compute the Test Statistic**

No population standard deviation is given, so we use the t-test:

$$t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}} = \frac{4.6 - 4}{1.2/\sqrt{35}} = \frac{0.6}{0.2028} = 2.958$$

**Step 4 — Critical Value and P-Value**

* Critical value (right-tailed, $\alpha = 0.05$, $DF = 34$): $t_c = 1.691$
* P-value: `tcdf(2.958, 1E99, 34)` $\approx 0.0028$

**Step 5 — Decision and Conclusion**

* Critical region: $t = 2.958 > t_c = 1.691$ → **Reject $H_0$**
* P-value: $p = 0.0028 \le \alpha = 0.05$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to support the claim that the average wait time for customers to receive their orders is more than 4 minutes.

[Return back to Lesson 20.5](../20_5_FullHypTests.md#practice)
