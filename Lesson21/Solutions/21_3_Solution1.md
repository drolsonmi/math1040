<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A pharmaceutical company claims that 70% of patients who take their medication experience significant improvement. A research group suspects the true rate is lower. In a clinical trial with a random sample of 150 patients, 96 experienced significant improvement. Conduct a full hypothesis test at the 5% significance level.

## Solution
From the problem:
* $$p_0 = 0.70$$, $$n = 150$$, $$x = 96$$, $$\hat{p} = 96/150 = 0.64$$
* $$\alpha = 0.05$$

**Step 1 — Verify the CLT**
* Random sample? **Yes**
* $$np_0 = 150(0.70) = 105 \ge 10$$ ✓ and $$n(1-p_0) = 150(0.30) = 45 \ge 10$$ ✓
* Independence: Population of potential patients is far greater than $$150 \times 10 = 1{,}500$$ ✓

**Step 2 — Hypotheses**

$$H_0: p = 0.70 \qquad\qquad H_A: p < 0.70 \quad \text{(left-tailed)}$$

**Step 3 — Test Statistic**

$$SE = \sqrt{\frac{0.70(0.30)}{150}} = \sqrt{0.0014} = 0.03742$$

$$z = \frac{0.64 - 0.70}{0.03742} = \frac{-0.06}{0.03742} = -1.603$$

**Step 4 — Critical Value and P-Value**

* Critical value (left-tailed, $$\alpha = 0.05$$): $$z_c = -1.645$$
* P-value: `normalcdf(-1E99, -1.603, 0, 1)` $$\approx 0.0545$$

**Step 5 — Decision and Conclusion**

* $$z = -1.603 > z_c = -1.645$$ → Test statistic is **not** in the critical region
* $$p = 0.0545 > \alpha = 0.05$$ → **Fail to reject $$H_0$$**

**Conclusion:** There is **not** sufficient evidence at the 5% significance level to conclude that the true rate of significant improvement is lower than the company's claimed 70%. (Note: the sample result of 64% is suggestive, but does not clear the 5% threshold.)

[Return back to Lesson 21.3](../21_3_FullCatHypTests.md#practice)
