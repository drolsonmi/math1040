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
2. A university reports that 30% of its students are first-generation college students. A student affairs office believes the proportion may be different. They survey a random sample of 250 students and find that 85 are first-generation students. At the 10% significance level, find the test statistic and the p-value.

## Solution
From Lesson 21.1 we have:
* $p_0 = 0.30$, $n = 250$, $x = 85$, $\hat{p} = 0.34$
* $H_0: p = 0.30 \qquad H_A: p \ne 0.30$ (two-tailed)
* CLT verified ✓

**Standard Error:**

$$SE = \sqrt{\frac{p_0(1-p_0)}{n}} = \sqrt{\frac{0.30(0.70)}{250}} = \sqrt{\frac{0.21}{250}} = \sqrt{0.00084} = 0.02898$$

**Test Statistic:**

$$z = \frac{\hat{p} - p_0}{SE} = \frac{0.34 - 0.30}{0.02898} = \frac{0.04}{0.02898} = 1.380$$

**Critical Value** (two-tailed, $\alpha = 0.10$): $z_c = \pm 1.645$

**P-value** (two-tailed):

$$p = 2 \times P(Z > 1.380)$$

On TI-84: `2 × normalcdf(1.380, 1E99, 0, 1)` $\approx 2 \times 0.0838 = 0.1676$

**Decision:**
* Critical region: $|z| = 1.380 < z_c = 1.645$ → Test statistic does **not** fall in the critical region
* P-value: $p = 0.1676 > \alpha = 0.10$ → **Fail to reject $H_0$**

**Conclusion:** There is **not** sufficient evidence at the 10% significance level to conclude that the proportion of first-generation students differs from 30%.

[Return back to Lesson 21.2](../21_2_CatCriticalAndP.md#practice)
