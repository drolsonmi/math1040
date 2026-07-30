<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A random sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level using the p-value method.

## Solution
From the problem we get the following information:
* Null value: $\mu_0 = 20$
* Sample size: $n = 55$, $DF = 54$
* Sample mean: $\bar{x} = 18.7$
* Sample standard deviation: $s = 2.5$
* Significance level: $\alpha = 0.01$

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes**
* Is $n \ge 30$? **Yes**

The CLT holds.

**Step 2 — State the hypotheses**

$$H_0: \mu = 20 \qquad\qquad H_A: \mu < 20 \quad \text{(left-tailed)}$$

**Step 3 — Compute the test statistic**

$$t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}} = \frac{18.7 - 20}{2.5/\sqrt{55}} = \frac{-1.3}{0.3370} = -3.858$$

**Step 4 — Find the p-value**

For a left-tailed t-test with $t = -3.858$ and $DF = 54$:

$$p = P(T < -3.858) \approx 0.0002$$

On the TI-84: `tcdf(-1E99, -3.858, 54)` $\approx 0.0002$

**Step 5 — Make a decision**

$$p = 0.0002 \le \alpha = 0.01$$

We **reject $H_0$**.

**Conclusion:** There is sufficient evidence at the 1% significance level to support the claim that the average battery life is less than 20 hours.

[Return back to Lesson 20.4](../20_4_PValues.md#practice)
