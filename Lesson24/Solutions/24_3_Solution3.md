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

1. A nutritionist wants to know if a 6-week diet program changes participants' weight, using $d = \text{Before} - \text{After}$ ($\bar{d} = 6.6$, $s_d \approx 1.517$, $n = 5$). Build a 95% confidence interval for $\mu_d$.

## Solution

From Lessons 24.1–24.2: $\bar{d} = 6.6$, $s_d \approx 1.517$, $n = 5$, conditions verified ✓.

Since this is a two-tailed test at $\alpha = 0.05$, we use a confidence level of $1-\alpha = 0.95$, or 95%.

**Standard Error:**

\[SE = \frac{1.517}{\sqrt{5}} \approx 0.6785\]

**Critical Value** ($df = 4$, 95% confidence): $t_c \approx 2.776$

**Confidence Interval:**

\[6.6 \pm 2.776(0.6785) = 6.6 \pm 1.883\]

\[(4.717, \ 8.483)\]

**Conclusion:** We are 95% confident that the true mean difference in weight before and after the diet program ($\mu_d$) is between 4.717 and 8.483 lbs. Since the entire interval is above 0, there is evidence that the diet program changes (reduces) participants' weight.

[Return back to Lesson 24.3](https://drolsonmi.github.io/math1040/Lesson24/24_3_ConfidenceIntervals.html#practice)
