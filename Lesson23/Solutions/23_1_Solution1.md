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

1. A marketing team wants to know if customer satisfaction differs between two products. A random sample of 180 Product A customers found 126 satisfied. An independent random sample of 165 Product B customers found 90 satisfied. Test at the 5% significance level.

## Solution

**Identifying the information:**

- Product A: $n_1 = 180$, $x_1 = 126$, so $\hat{p}_1 = 126/180 = 0.70$
- Product B: $n_2 = 165$, $x_2 = 90$, so $\hat{p}_2 = 90/165 \approx 0.545$

**Hypotheses:**

\[H_0: p_1 = p_2 \qquad\qquad H_A: p_1 \ne p_2 \quad \text{(two-tailed)}\]

**Verify the Conditions:**

- Both samples are random — *stated in the problem*
- The two samples are independent — *different customers for each product*
- Pooled proportion: $\bar{p} = \dfrac{126+90}{180+165} = \dfrac{216}{345} \approx 0.626$
  * $n_1\bar{p} = 180(0.626) = 112.7 \ge 10$ ✓ and $n_1(1-\bar{p}) = 180(0.374) = 67.3 \ge 10$ ✓
  * $n_2\bar{p} = 165(0.626) = 103.3 \ge 10$ ✓ and $n_2(1-\bar{p}) = 165(0.374) = 61.7 \ge 10$ ✓

All conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 23.1](https://drolsonmi.github.io/math1040/Lesson23/23_1_Hypotheses.html#practice)
