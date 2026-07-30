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

1. An education researcher wants to know if there is a difference in average test scores between School A and School B. A random sample of 40 students at School A had an average score of 78.4 with a standard deviation of 8.2. An independent random sample of 38 students at School B had an average score of 74.9 with a standard deviation of 7.5. Conduct a full hypothesis test at the 5% significance level (use $df \approx 75.7$).

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes**
- Independent? **Yes** — different students at two different schools
- Large enough? $n_1 = 40 \ge 30$ ✓ and $n_2 = 38 \ge 30$ ✓

**Step 2 — Hypotheses**

\[H_0: \mu_1 = \mu_2 \qquad\qquad H_A: \mu_1 \ne \mu_2 \quad \text{(two-tailed)}\]

**Step 3 — Test Statistic**

\[SE = \sqrt{\frac{8.2^2}{40}+\frac{7.5^2}{38}} \approx 1.778\]

\[t = \frac{78.4-74.9}{1.778} = \frac{3.5}{1.778} \approx 1.968\]

**Step 4 — Critical Value and P-Value**

- Critical value (two-tailed, $\alpha = 0.05$, $df \approx 75.7$): $t_c \approx \pm 1.992$
- P-value: $p \approx 0.053$

**Step 5 — Decision and Conclusion**

- $|t| = 1.968 < t_c = 1.992$ → **Fail to reject $H_0$**
- $p \approx 0.053 > \alpha = 0.05$ → **Fail to reject $H_0$**

**Conclusion:** There is not sufficient evidence at the 5% significance level to conclude that the average test scores are different between School A and School B.

[Return back to Lesson 22.4](https://drolsonmi.github.io/math1040/Lesson22/22_4_HypothesisTest.html#practice)
