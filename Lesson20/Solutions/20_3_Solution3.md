<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. A random sample of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level.

## Solution
From the problem we get the following information:
* Null value: $$\mu_0 = 75$$
* Sample size: $$n = 40$$
* Sample mean: $$\bar{x} = 78.2$$
* Sample standard deviation: $$s = 6.3$$
* Significance level: $$\alpha = 0.05$$

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes** (stated in this version of the problem)
* Is the sample large enough? **Yes** ($$n = 40 \ge 30$$)

The Central Limit Theorem holds.

**Step 2 — State the hypotheses**

We are testing whether the new method leads to a **different** average score — not specifically higher or lower.

$$H_0: \mu = 75 \qquad\qquad H_A: \mu \ne 75 \quad \text{(two-tailed)}$$

**Step 3 — Find the critical value**

For a two-tailed test with $$\alpha = 0.05$$ and $$DF = n - 1 = 39$$ degrees of freedom, each tail contains $$\alpha/2 = 0.025$$. The critical t-value is:

$$t_c = \pm 2.023$$

**Step 4 — Compute the test statistic**

$$t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}} = \frac{78.2 - 75}{6.3/\sqrt{40}} = \frac{3.2}{0.9963} = 3.212$$

**Step 5 — Make a decision**

$$|t| = 3.212 > t_c = 2.023$$

The test statistic falls in the critical region, so we **reject $$H_0$$**.

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the new teaching method leads to a different average score than 75.

[Return back to Lesson 20.3](../20_3_CriticalRegions.md#practice)
