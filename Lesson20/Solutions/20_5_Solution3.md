<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
3. A hospital administrator claims the average length of stay for patients after a routine surgery is 3.5 days. A quality-improvement team suspects the average may be different. They review a random sample of 45 patient records and find a mean stay of 3.9 days with a standard deviation of 1.1 days. Conduct a full hypothesis test at the 5% significance level.

## Solution
From the problem we get the following information:
* Null value: $$\mu_0 = 3.5$$
* Sample size: $$n = 45$$, $$DF = 44$$
* Sample mean: $$\bar{x} = 3.9$$
* Sample standard deviation: $$s = 1.1$$
* Significance level: $$\alpha = 0.05$$

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes** (stated in the problem)
* Is $$n \ge 30$$? **Yes** ($$n = 45$$)

The CLT holds.

**Step 2 — State the Hypotheses**

The team suspects the average may be **different** from 3.5 days — either direction.

$$H_0: \mu = 3.5 \qquad\qquad H_A: \mu \ne 3.5 \quad \text{(two-tailed)}$$

**Step 3 — Compute the Test Statistic**

$$t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}} = \frac{3.9 - 3.5}{1.1/\sqrt{45}} = \frac{0.4}{0.1640} = 2.439$$

**Step 4 — Critical Value and P-Value**

* Critical value (two-tailed, $$\alpha = 0.05$$, $$DF = 44$$): $$t_c = \pm 2.015$$
* P-value: `2 × tcdf(2.439, 1E99, 44)` $$\approx 2 \times 0.0092 = 0.0184$$

**Step 5 — Decision and Conclusion**

* Critical region: $$|t| = 2.439 > t_c = 2.015$$ → **Reject $$H_0$$**
* P-value: $$p = 0.0184 \le \alpha = 0.05$$ → **Reject $$H_0$$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the average length of hospital stay after routine surgery is different from the claimed 3.5 days.

[Return back to Lesson 20.5](../20_5_FullHypTests.md#practice)
