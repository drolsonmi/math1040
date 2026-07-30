<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. A random sample of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level using the p-value method.

## Solution
From the problem we get the following information:
* Null value: $\mu_0 = 75$
* Sample size: $n = 40$, $DF = 39$
* Sample mean: $\bar{x} = 78.2$
* Sample standard deviation: $s = 6.3$
* Significance level: $\alpha = 0.05$

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes**
* Is $n \ge 30$? **Yes**

The CLT holds.

**Step 2 — State the hypotheses**

$$H_0: \mu = 75 \qquad\qquad H_A: \mu \ne 75 \quad \text{(two-tailed)}$$

**Step 3 — Compute the test statistic**

$$t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}} = \frac{78.2 - 75}{6.3/\sqrt{40}} = \frac{3.2}{0.9963} = 3.212$$

**Step 4 — Find the p-value**

For a two-tailed t-test with $|t| = 3.212$ and $DF = 39$:

$$p = 2 \times P(T > 3.212) \approx 2 \times 0.0013 = 0.0026$$

On the TI-84: `2 × tcdf(3.212, 1E99, 39)` $\approx 0.0026$

**Step 5 — Make a decision**

$$p = 0.0026 \le \alpha = 0.05$$

We **reject $H_0$**.

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the new teaching method leads to a different average score than 75.

[Return back to Lesson 20.4](../20_4_PValues.md#practice)
