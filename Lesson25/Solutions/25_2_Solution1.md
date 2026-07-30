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

1. A business analyst wants to know if there's a positive relationship between advertising spend and sales revenue. A random sample of 15 months shows a sample correlation of $r = 0.68$. Conduct a full hypothesis test at the 5% significance level.

## Solution

From Lesson 25.1: $H_0: \rho = 0$, $H_A: \rho > 0$ (right-tailed), conditions verified ✓.

**Test Statistic:**

$$t = \frac{0.68\sqrt{15-2}}{\sqrt{1-0.68^2}} = \frac{0.68\sqrt{13}}{\sqrt{0.5376}} = \frac{2.452}{0.733} \approx 3.344 \qquad df = 13$$

**Critical Value** (right-tailed, $\alpha = 0.05$, $df = 13$): $t_c \approx 1.771$

**P-value:** $p \approx 0.0026$

**Decision:** $t = 3.344 > t_c = 1.771$ (and $p \approx 0.0026 \le \alpha = 0.05$) → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that there is a positive linear relationship between advertising spend and sales revenue.

[Return back to Lesson 25.2](https://drolsonmi.github.io/math1040/Lesson25/25_2_TestingCorrelation.html#practice)
