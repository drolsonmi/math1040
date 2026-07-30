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

1. A researcher tests whether caffeine improves (lowers) reaction time, using $d = \text{Before} - \text{After}$ ($\bar{d} = 17.2$, $s_d \approx 8.928$, $n = 5$). Build a 90% confidence interval for $\mu_d$.

## Solution

From Lessons 24.1–24.2: $\bar{d} = 17.2$, $s_d \approx 8.928$, $n = 5$, conditions verified ✓.

Since this interval corresponds to the one-tailed test ($\alpha = 0.05$) from Lesson 24.2, we use a confidence level of $1-2\alpha = 0.90$, or 90%.

**Standard Error:**

\[SE = \frac{8.928}{\sqrt{5}} \approx 3.9927\]

**Critical Value** ($df = 4$, 90% confidence): $t_c \approx 2.132$

**Confidence Interval:**

\[17.2 \pm 2.132(3.9927) = 17.2 \pm 8.512\]

\[(8.688, \ 25.712)\]

**Conclusion:** We are 90% confident that the true mean reduction in reaction time after drinking caffeine ($\mu_d$) is between 8.688 and 25.712 milliseconds. Since the entire interval is above 0, there is evidence that caffeine lowers reaction time.

[Return back to Lesson 24.3](https://drolsonmi.github.io/math1040/Lesson24/24_3_ConfidenceIntervals.html#practice)
