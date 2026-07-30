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

1. A nutritionist wants to know if a 6-week diet program changes participants' weight, using $d = \text{Before} - \text{After}$ ($\bar{d} = 6.6$, $s_d \approx 1.517$, $n = 5$). Test at the 5% significance level.

## Solution

**Hypotheses:**

The nutritionist only wants to know if weight **changes** — not specifically whether it increases or decreases — so this is a two-tailed test.

\[H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d \ne 0 \quad \text{(two-tailed)}\]

**Verify the Conditions:**

- The sample is random — *assumed from the study description*
- The sample size is small ($n = 5 < 30$), so we need the differences to be approximately normal. The 5 differences (5, 5, 7, 8, 8) are tightly clustered with no extreme outliers, so we'll treat this condition as satisfied.

Both conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 24.2](https://drolsonmi.github.io/math1040/Lesson24/24_2_Hypotheses.html#practice)
