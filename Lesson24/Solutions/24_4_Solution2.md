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

1. An instructor wants to know if a review session improves (raises) exam scores, using $d = \text{Posttest} - \text{Pretest}$ ($\bar{d} \approx 3.833$, $s_d \approx 2.787$, $n = 6$). Conduct a full hypothesis test at the 1% significance level.

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes** (assumed from study description)
- $n = 6 < 30$, but the differences show no extreme outliers, so we treat the normality condition as satisfied

**Step 2 — Hypotheses**

\[H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d > 0 \quad \text{(right-tailed)}\]

**Step 3 — Test Statistic**

\[SE = \frac{2.787}{\sqrt{6}} \approx 1.1379\]

\[t = \frac{3.833 - 0}{1.1379} \approx 3.369 \qquad\qquad df = 5\]

**Step 4 — Critical Value and P-Value**

- Critical value (right-tailed, $\alpha = 0.01$, $df = 5$): $t_c \approx 3.365$
- P-value: $p \approx 0.0099$

**Step 5 — Decision and Conclusion**

- $t = 3.369 > t_c = 3.365$ → **Reject $H_0$** (very close call!)
- $p \approx 0.0099 \le \alpha = 0.01$ → **Reject $H_0$** (also very close!)

**Conclusion:** There is sufficient evidence at the 1% significance level to conclude that the review session raises exam scores — though just barely.

[Return back to Lesson 24.4](https://drolsonmi.github.io/math1040/Lesson24/24_4_HypothesisTest.html#practice)
