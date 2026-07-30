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

1. A researcher wants to know if more screen time is associated with less sleep. A random sample of 20 teenagers shows a sample correlation of $r = -0.45$ between daily screen time and hours of sleep. Conduct a full hypothesis test at the 1% significance level.

## Solution

From Lesson 25.1: $H_0: \rho = 0$, $H_A: \rho < 0$ (left-tailed), conditions verified ✓.

**Test Statistic:**

$$t = \frac{-0.45\sqrt{20-2}}{\sqrt{1-(-0.45)^2}} = \frac{-0.45\sqrt{18}}{\sqrt{0.7975}} = \frac{-1.909}{0.893} \approx -2.138 \qquad df = 18$$

**Critical Value** (left-tailed, $\alpha = 0.01$, $df = 18$): $t_c \approx -2.552$

**P-value:** $p \approx 0.0233$

**Decision:** $t = -2.138 > t_c = -2.552$, so the test statistic is **not** in the critical region (and $p \approx 0.0233 > \alpha = 0.01$) → **Fail to reject $H_0$**

**Conclusion:** There is not sufficient evidence at the 1% significance level to conclude that more screen time is associated with less sleep.

[Return back to Lesson 25.2](https://drolsonmi.github.io/math1040/Lesson25/25_2_TestingCorrelation.html#practice)
