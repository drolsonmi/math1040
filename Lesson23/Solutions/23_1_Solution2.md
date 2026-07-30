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

1. A public health department wants to know if a new smoking cessation program has a higher success rate than the standard program. A random sample of 140 participants in the new program found that 42 successfully quit smoking. An independent random sample of 150 participants in the standard program found that 27 successfully quit. Test at the 1% significance level.

## Solution

**Identifying the information:**

- New program: $n_1 = 140$, $x_1 = 42$, so $\hat{p}_1 = 42/140 = 0.30$
- Standard program: $n_2 = 150$, $x_2 = 27$, so $\hat{p}_2 = 27/150 = 0.18$

**Hypotheses:**

We are testing whether the new program's success rate is **higher**.

\[H_0: p_1 = p_2 \qquad\qquad H_A: p_1 > p_2 \quad \text{(right-tailed)}\]

**Verify the Conditions:**

- Both samples are random — *stated in the problem*
- The two samples are independent — *different participants in each program*
- Pooled proportion: $\bar{p} = \dfrac{42+27}{140+150} = \dfrac{69}{290} \approx 0.238$
  * $n_1\bar{p} = 140(0.238) = 33.3 \ge 10$ ✓ and $n_1(1-\bar{p}) = 140(0.762) = 106.7 \ge 10$ ✓
  * $n_2\bar{p} = 150(0.238) = 35.7 \ge 10$ ✓ and $n_2(1-\bar{p}) = 150(0.762) = 114.3 \ge 10$ ✓

All conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 23.1](https://drolsonmi.github.io/math1040/Lesson23/23_1_Hypotheses.html#practice)
