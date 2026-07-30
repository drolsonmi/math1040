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

1. A nutritionist wants to know if a 6-week diet program changes participants' weight, using $d = \text{Before} - \text{After}$ ($\bar{d} = 6.6$, $s_d \approx 1.517$, $n = 5$). Conduct a full hypothesis test at the 5% significance level.

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes** (assumed from study description)
- $n = 5 < 30$, but the differences show no extreme outliers, so we treat the normality condition as satisfied

**Step 2 — Hypotheses**

\[H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d \ne 0 \quad \text{(two-tailed)}\]

**Step 3 — Test Statistic**

\[SE = \frac{1.517}{\sqrt{5}} \approx 0.6785\]

\[t = \frac{6.6 - 0}{0.6785} \approx 9.727 \qquad\qquad df = 4\]

**Step 4 — Critical Value and P-Value**

- Critical value (two-tailed, $\alpha = 0.05$, $df = 4$): $t_c \approx \pm 2.776$
- P-value: $p \approx 0.0006$

**Step 5 — Decision and Conclusion**

- $t = 9.727 > t_c = 2.776$ → **Reject $H_0$**
- $p \approx 0.0006 \le \alpha = 0.05$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that participants' weight changes over the course of the 6-week diet program.

[Return back to Lesson 24.4](https://drolsonmi.github.io/math1040/Lesson24/24_4_HypothesisTest.html#practice)
