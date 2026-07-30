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

1. A quality control manager wants to know if Machine A has a lower defect rate than Machine B. A random sample of 200 items from Machine A found 14 defective. An independent random sample of 220 items from Machine B found 24 defective. Conduct a full hypothesis test at the 5% significance level.

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes**
- Independent? **Yes** — different items from two different machines
- Pooled proportion: $\bar{p} = \dfrac{14+24}{200+220} \approx 0.090$; all four success-failure checks pass (see Lesson 23.1) ✓

**Step 2 — Hypotheses**

\[H_0: p_1 = p_2 \qquad\qquad H_A: p_1 < p_2 \quad \text{(left-tailed)}\]

**Step 3 — Test Statistic**

\[\hat{p}_1 = 0.07 \qquad \hat{p}_2 \approx 0.109\]

\[SE = \sqrt{0.090(0.910)\left(\frac{1}{200}+\frac{1}{220}\right)} \approx 0.02803\]

\[z = \frac{0.07-0.109}{0.02803} = \frac{-0.039}{0.02803} \approx -1.391\]

**Step 4 — Critical Value and P-Value**

- Critical value (left-tailed, $\alpha = 0.05$): $z_c = -1.645$
- P-value: $p = P(Z < -1.391) \approx 0.0821$

**Step 5 — Decision and Conclusion**

- $z = -1.391 > z_c = -1.645$ (not in the critical region) → **Fail to reject $H_0$**
- $p \approx 0.0821 > \alpha = 0.05$ → **Fail to reject $H_0$**

**Conclusion:** There is not sufficient evidence at the 5% significance level to conclude that Machine A has a lower defect rate than Machine B.

[Return back to Lesson 23.3](https://drolsonmi.github.io/math1040/Lesson23/23_3_HypothesisTest.html#practice)
