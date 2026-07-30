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

1. An instructor wants to know if a review session improves (raises) exam scores, using $d = \text{Posttest} - \text{Pretest}$ ($\bar{d} \approx 3.833$, $s_d \approx 2.787$, $n = 6$). Test at the 1% significance level.

## Solution

**Hypotheses:**

If the review session raises scores, Posttest should be larger than Pretest, so $d$ should tend to be **positive**.

\[H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d > 0 \quad \text{(right-tailed)}\]

**Verify the Conditions:**

- The sample is random — *assumed from the study description*
- The sample size is small ($n = 6 < 30$), so we need the differences to be approximately normal. The 6 differences (-1, 3, 4, 4, 6, 7) are reasonably clustered with no extreme outliers, so we'll treat this condition as satisfied.

Both conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 24.2](https://drolsonmi.github.io/math1040/Lesson24/24_2_Hypotheses.html#practice)
