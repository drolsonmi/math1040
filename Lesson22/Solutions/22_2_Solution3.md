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

1. A transit planner wants to know if Bus Route 1 has a shorter average travel time than Bus Route 2. A random sample of 30 trips on Route 1 averaged 22.5 minutes with a standard deviation of 4.0 minutes. An independent random sample of 32 trips on Route 2 averaged 25.1 minutes with a standard deviation of 4.6 minutes. Test at the 5% significance level.

## Solution

**Identifying the information:**

- Route 1: $n_1 = 30$, $\bar{x}_1 = 22.5$, $s_1 = 4.0$
- Route 2: $n_2 = 32$, $\bar{x}_2 = 25.1$, $s_2 = 4.6$

**Hypotheses:**

We are testing whether Route 1 has a **shorter** (smaller) average travel time than Route 2.

\[H_0: \mu_1 = \mu_2 \qquad\qquad H_A: \mu_1 < \mu_2 \quad \text{(left-tailed)}\]

**Verify the Conditions:**

- Both samples are random — *stated in the problem*
- The two samples are independent — *different trips on two different routes*
- Both samples are large enough: $n_1 = 30 \ge 30$ ✓ and $n_2 = 32 \ge 30$ ✓

All conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 22.2](https://drolsonmi.github.io/math1040/Lesson22/22_2_Hypotheses.html#practice)
