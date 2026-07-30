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

1. A marketing team wants to know if customer satisfaction differs between two products. A random sample of 180 Product A customers found 126 satisfied. An independent random sample of 165 Product B customers found 90 satisfied. Conduct a full hypothesis test at the 5% significance level.

## Solution

**Step 1 — Verify the Conditions**

- Random? **Yes**
- Independent? **Yes** — different customers for each product
- Pooled proportion: $\bar{p} = \dfrac{126+90}{180+165} \approx 0.626$; all four success-failure checks pass (see Lesson 23.1) ✓

**Step 2 — Hypotheses**

\[H_0: p_1 = p_2 \qquad\qquad H_A: p_1 \ne p_2 \quad \text{(two-tailed)}\]

**Step 3 — Test Statistic**

\[\hat{p}_1 = 0.70 \qquad \hat{p}_2 \approx 0.545\]

\[SE = \sqrt{0.626(0.374)\left(\frac{1}{180}+\frac{1}{165}\right)} \approx 0.05215\]

\[z = \frac{0.70-0.545}{0.05215} = \frac{0.155}{0.05215} \approx 2.972\]

**Step 4 — Critical Value and P-Value**

- Critical value (two-tailed, $\alpha = 0.05$): $z_c = \pm 1.960$
- P-value: $p = 2 \times P(Z > 2.972) \approx 2 \times 0.00148 = 0.00296$

**Step 5 — Decision and Conclusion**

- $|z| = 2.972 > z_c = 1.960$ → **Reject $H_0$**
- $p \approx 0.003 \le \alpha = 0.05$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that customer satisfaction is different between Product A and Product B.

[Return back to Lesson 23.3](https://drolsonmi.github.io/math1040/Lesson23/23_3_HypothesisTest.html#practice)
