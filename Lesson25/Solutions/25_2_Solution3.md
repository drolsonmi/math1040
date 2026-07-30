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

1. An economist wants to know if there is any linear relationship at all between daily temperature and ice cream sales. A random sample of 30 days shows a sample correlation of $r = 0.39$. Conduct a full hypothesis test at the 5% significance level.

## Solution

From Lesson 25.1: $H_0: \rho = 0$, $H_A: \rho \ne 0$ (two-tailed), conditions verified ✓.

**Test Statistic:**

$$t = \frac{0.39\sqrt{30-2}}{\sqrt{1-0.39^2}} = \frac{0.39\sqrt{28}}{\sqrt{0.8479}} = \frac{2.064}{0.921} \approx 2.241 \qquad df = 28$$

**Critical Value** (two-tailed, $\alpha = 0.05$, $df = 28$): $t_c \approx \pm 2.048$

**P-value:** $p \approx 0.0332$

**Decision:** $|t| = 2.241 > t_c = 2.048$ (and $p \approx 0.0332 \le \alpha = 0.05$) → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that there is a linear relationship between daily temperature and ice cream sales.

[Return back to Lesson 25.2](https://drolsonmi.github.io/math1040/Lesson25/25_2_TestingCorrelation.html#practice)
