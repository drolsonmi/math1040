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

1. A public health department wants to know if a new smoking cessation program has a higher success rate than the standard program. A random sample of 140 participants in the new program found that 42 successfully quit smoking. An independent random sample of 150 participants in the standard program found that 27 successfully quit. Conduct a full hypothesis test at the 1% significance level.

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes**
- Independent? **Yes** — different participants in each program
- Pooled proportion: $\bar{p} = \dfrac{42+27}{140+150} \approx 0.238$; all four success-failure checks pass (see Lesson 23.1) ✓

**Step 2 — Hypotheses**

\[H_0: p_1 = p_2 \qquad\qquad H_A: p_1 > p_2 \quad \text{(right-tailed)}\]

**Step 3 — Test Statistic**

\[\hat{p}_1 = 0.30 \qquad \hat{p}_2 = 0.18\]

\[SE = \sqrt{0.238(0.762)\left(\frac{1}{140}+\frac{1}{150}\right)} \approx 0.05004\]

\[z = \frac{0.30-0.18}{0.05004} = \frac{0.12}{0.05004} \approx 2.398\]

**Step 4 — Critical Value and P-Value**

- Critical value (right-tailed, $\alpha = 0.01$): $z_c = 2.326$
- P-value: $p = P(Z > 2.398) \approx 0.0082$

**Step 5 — Decision and Conclusion**

- $z = 2.398 > z_c = 2.326$ → **Reject $H_0$**
- $p \approx 0.0082 \le \alpha = 0.01$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 1% significance level to conclude that the new smoking cessation program has a higher success rate than the standard program.

[Return back to Lesson 23.3](https://drolsonmi.github.io/math1040/Lesson23/23_3_HypothesisTest.html#practice)
