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

1. A researcher tests whether caffeine improves (lowers) reaction time, using $d = \text{Before} - \text{After}$ ($\bar{d} = 17.2$, $s_d \approx 8.928$, $n = 5$). Test at the 5% significance level.

## Solution

**Hypotheses:**

If caffeine lowers reaction time, Before should be larger than After, so $d$ should tend to be **positive**.

\[H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d > 0 \quad \text{(right-tailed)}\]

**Verify the Conditions:**

- The sample is random — *assumed from the study description*
- The sample size is small ($n = 5 < 30$), so we need the differences to be approximately normal. The 5 differences (10, 10, 13, 23, 30) don't show any extreme outliers, so we'll treat this condition as reasonably satisfied, though a sample this small gives us limited ability to check.

Both conditions are satisfied. We can proceed with the hypothesis test.

[Return back to Lesson 24.2](https://drolsonmi.github.io/math1040/Lesson24/24_2_Hypotheses.html#practice)
