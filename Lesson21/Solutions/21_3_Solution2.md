<head>
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

## Practice
2. A university reports that 30% of its students are first-generation college students. A student affairs office believes the proportion may be different. They survey a random sample of 250 students and find 85 are first-generation students. Conduct a full hypothesis test at the 10% significance level.

## Solution
From the problem:
* $p_0 = 0.30$, $n = 250$, $x = 85$, $\hat{p} = 85/250 = 0.34$
* $\alpha = 0.10$

**Step 1 — Verify the CLT**
* Random sample? **Yes**
* $np_0 = 250(0.30) = 75 \ge 10$ ✓ and $n(1-p_0) = 250(0.70) = 175 \ge 10$ ✓
* Independence: The university has far more than $250 \times 10 = 2{,}500$ students ✓

**Step 2 — Hypotheses**

$$H_0: p = 0.30 \qquad\qquad H_A: p \ne 0.30 \quad \text{(two-tailed)}$$

**Step 3 — Test Statistic**

$$SE = \sqrt{\frac{0.30(0.70)}{250}} = \sqrt{0.00084} = 0.02898$$

$$z = \frac{0.34 - 0.30}{0.02898} = \frac{0.04}{0.02898} = 1.380$$

**Step 4 — Critical Value and P-Value**

* Critical value (two-tailed, $\alpha = 0.10$): $z_c = \pm 1.645$
* P-value: `2 × normalcdf(1.380, 1E99, 0, 1)` $\approx 2 \times 0.0838 = 0.1676$

**Step 5 — Decision and Conclusion**

* $|z| = 1.380 < z_c = 1.645$ → Test statistic is **not** in the critical region
* $p = 0.1676 > \alpha = 0.10$ → **Fail to reject $H_0$**

**Conclusion:** There is **not** sufficient evidence at the 10% significance level to conclude that the proportion of first-generation college students differs from 30%.

[Return back to Lesson 21.3](../21_3_FullCatHypTests.md#practice)
