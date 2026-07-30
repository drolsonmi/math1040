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

1. A fitness researcher wants to know if Program X leads to greater average weight loss than Program Y. A random sample of 25 participants using Program X lost an average of 12.3 lbs with a standard deviation of 3.1 lbs. An independent random sample of 28 participants using Program Y lost an average of 9.8 lbs with a standard deviation of 2.8 lbs. Conduct a full hypothesis test at the 1% significance level (use $df \approx 49.8$).

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes**
- Independent? **Yes** — different participants in each program
- Large enough? $n_1 = 25 < 30$ and $n_2 = 28 < 30$. Neither reaches 30, so we assume weight loss is approximately normally distributed in each population.

**Step 2 — Hypotheses**

\[H_0: \mu_1 = \mu_2 \qquad\qquad H_A: \mu_1 > \mu_2 \quad \text{(right-tailed)}\]

**Step 3 — Test Statistic**

\[SE = \sqrt{\frac{3.1^2}{25}+\frac{2.8^2}{28}} \approx 0.8151\]

\[t = \frac{12.3-9.8}{0.8151} = \frac{2.5}{0.8151} \approx 3.067\]

**Step 4 — Critical Value and P-Value**

- Critical value (right-tailed, $\alpha = 0.01$, $df \approx 49.8$): $t_c \approx 2.403$
- P-value: $p \approx 0.0017$

**Step 5 — Decision and Conclusion**

- $t = 3.067 > t_c = 2.403$ → **Reject $H_0$**
- $p \approx 0.0017 \le \alpha = 0.01$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 1% significance level to conclude that Program X leads to greater average weight loss than Program Y.

[Return back to Lesson 22.4](https://drolsonmi.github.io/math1040/Lesson22/22_4_HypothesisTest.html#practice)
