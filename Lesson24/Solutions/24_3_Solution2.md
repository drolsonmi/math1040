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

1. An instructor wants to know if a review session improves (raises) exam scores, using $d = \text{Posttest} - \text{Pretest}$ ($\bar{d} \approx 3.833$, $s_d \approx 2.787$, $n = 6$). Build a 98% confidence interval for $\mu_d$.

## Solution

From Lessons 24.1–24.2: $\bar{d} \approx 3.833$, $s_d \approx 2.787$, $n = 6$, conditions verified ✓.

Since this interval corresponds to the one-tailed test ($\alpha = 0.01$) from Lesson 24.2, we use a confidence level of $1-2\alpha = 0.98$, or 98%.

**Standard Error:**

\[SE = \frac{2.787}{\sqrt{6}} \approx 1.1379\]

**Critical Value** ($df = 5$, 98% confidence): $t_c \approx 3.365$

**Confidence Interval:**

\[3.833 \pm 3.365(1.1379) = 3.833 \pm 3.829\]

\[(0.004, \ 7.662)\]

**Conclusion:** We are 98% confident that the true mean increase in exam scores after the review session ($\mu_d$) is between 0.004 and 7.662 points. Since the entire interval is above 0 (barely!), there is evidence that the review session raises exam scores.

[Return back to Lesson 24.3](https://drolsonmi.github.io/math1040/Lesson24/24_3_ConfidenceIntervals.html#practice)
