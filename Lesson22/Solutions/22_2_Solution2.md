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

1. A fitness researcher wants to know if Program X leads to greater average weight loss than Program Y. A random sample of 25 participants using Program X lost an average of 12.3 lbs with a standard deviation of 3.1 lbs. An independent random sample of 28 participants using Program Y lost an average of 9.8 lbs with a standard deviation of 2.8 lbs. Test at the 1% significance level.

## Solution

**Identifying the information:**

- Program X: $n_1 = 25$, $\bar{x}_1 = 12.3$, $s_1 = 3.1$
- Program Y: $n_2 = 28$, $\bar{x}_2 = 9.8$, $s_2 = 2.8$

**Hypotheses:**

We are testing whether Program X leads to **greater** weight loss than Program Y.

\[H_0: \mu_1 = \mu_2 \qquad\qquad H_A: \mu_1 > \mu_2 \quad \text{(right-tailed)}\]

**Verify the Conditions:**

- Both samples are random — *stated in the problem*
- The two samples are independent — *different participants in each program*
- Both samples are large enough: $n_1 = 25 < 30$ and $n_2 = 28 < 30$. Neither sample reaches 30, so we need to assume weight loss is approximately normally distributed in each population — a reasonable assumption for this type of measurement.

With that assumption, all conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 22.2](https://drolsonmi.github.io/math1040/Lesson22/22_2_Hypotheses.html#practice)
