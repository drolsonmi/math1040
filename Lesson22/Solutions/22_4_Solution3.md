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

1. A transit planner wants to know if Bus Route 1 has a shorter average travel time than Bus Route 2. A random sample of 30 trips on Route 1 averaged 22.5 minutes with a standard deviation of 4.0 minutes. An independent random sample of 32 trips on Route 2 averaged 25.1 minutes with a standard deviation of 4.6 minutes. Conduct a full hypothesis test at the 5% significance level (use $df \approx 59.5$).

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes**
- Independent? **Yes** — different trips on two different routes
- Large enough? $n_1 = 30 \ge 30$ ✓ and $n_2 = 32 \ge 30$ ✓

**Step 2 — Hypotheses**

\[H_0: \mu_1 = \mu_2 \qquad\qquad H_A: \mu_1 < \mu_2 \quad \text{(left-tailed)}\]

**Step 3 — Test Statistic**

\[SE = \sqrt{\frac{4.0^2}{30}+\frac{4.6^2}{32}} \approx 1.0930\]

\[t = \frac{22.5-25.1}{1.0930} = \frac{-2.6}{1.0930} \approx -2.379\]

**Step 4 — Critical Value and P-Value**

- Critical value (left-tailed, $\alpha = 0.05$, $df \approx 59.5$): $t_c \approx -1.671$
- P-value: $p \approx 0.0103$

**Step 5 — Decision and Conclusion**

- $t = -2.379 < t_c = -1.671$ → **Reject $H_0$**
- $p \approx 0.0103 \le \alpha = 0.05$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that Bus Route 1 has a shorter average travel time than Bus Route 2.

[Return back to Lesson 22.4](https://drolsonmi.github.io/math1040/Lesson22/22_4_HypothesisTest.html#practice)
