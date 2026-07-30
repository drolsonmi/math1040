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

1. A quality control manager wants to know if Machine A has a lower defect rate than Machine B. A random sample of 200 items from Machine A found 14 defective. An independent random sample of 220 items from Machine B found 24 defective. Test at the 5% significance level.

## Solution

**Identifying the information:**

- Machine A: $n_1 = 200$, $x_1 = 14$, so $\hat{p}_1 = 14/200 = 0.07$
- Machine B: $n_2 = 220$, $x_2 = 24$, so $\hat{p}_2 = 24/220 \approx 0.109$

**Hypotheses:**

We are testing whether Machine A's defect rate is **lower**.

\[H_0: p_1 = p_2 \qquad\qquad H_A: p_1 < p_2 \quad \text{(left-tailed)}\]

**Verify the Conditions:**

- Both samples are random — *stated in the problem*
- The two samples are independent — *different items from two different machines*
- Pooled proportion: $\bar{p} = \dfrac{14+24}{200+220} = \dfrac{38}{420} \approx 0.090$
  * $n_1\bar{p} = 200(0.090) = 18.1 \ge 10$ ✓ and $n_1(1-\bar{p}) = 200(0.910) = 182.0 \ge 10$ ✓
  * $n_2\bar{p} = 220(0.090) = 19.9 \ge 10$ ✓ and $n_2(1-\bar{p}) = 220(0.910) = 200.1 \ge 10$ ✓

All conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 23.1](https://drolsonmi.github.io/math1040/Lesson23/23_1_Hypotheses.html#practice)
