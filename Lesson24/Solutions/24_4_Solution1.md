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

1. A researcher tests whether caffeine improves (lowers) reaction time, using $d = \text{Before} - \text{After}$ ($\bar{d} = 17.2$, $s_d \approx 8.928$, $n = 5$). Conduct a full hypothesis test at the 5% significance level.

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes** (assumed from study description)
- $n = 5 < 30$, but the differences show no extreme outliers, so we treat the normality condition as satisfied

**Step 2 — Hypotheses**

\[H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d > 0 \quad \text{(right-tailed)}\]

**Step 3 — Test Statistic**

\[SE = \frac{8.928}{\sqrt{5}} \approx 3.9927\]

\[t = \frac{17.2 - 0}{3.9927} \approx 4.308 \qquad\qquad df = 4\]

**Step 4 — Critical Value and P-Value**

- Critical value (right-tailed, $\alpha = 0.05$, $df = 4$): $t_c \approx 2.132$
- P-value: $p \approx 0.0063$

**Step 5 — Decision and Conclusion**

- $t = 4.308 > t_c = 2.132$ → **Reject $H_0$**
- $p \approx 0.0063 \le \alpha = 0.05$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that caffeine lowers reaction time.

[Return back to Lesson 24.4](https://drolsonmi.github.io/math1040/Lesson24/24_4_HypothesisTest.html#practice)
