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

1. A transit planner wants to know if Bus Route 1 has a shorter average travel time than Bus Route 2. A random sample of 30 trips on Route 1 averaged 22.5 minutes with a standard deviation of 4.0 minutes. An independent random sample of 32 trips on Route 2 averaged 25.1 minutes with a standard deviation of 4.6 minutes. Build a 90% confidence interval for $\mu_1 - \mu_2$ (use $df \approx 59.5$).

## Solution

From Lesson 22.2 we have:

- $n_1 = 30$, $\bar{x}_1 = 22.5$, $s_1 = 4.0$
- $n_2 = 32$, $\bar{x}_2 = 25.1$, $s_2 = 4.6$
- Conditions verified ✓

Since this is ultimately headed toward a left-tailed test at $\alpha = 0.05$, we use a two-sided confidence level of $1-2\alpha = 0.90$, or 90%.

**Point Estimate:**

\[\bar{x}_1 - \bar{x}_2 = 22.5 - 25.1 = -2.6\]

**Standard Error:**

\[SE = \sqrt{\frac{4.0^2}{30}+\frac{4.6^2}{32}} = \sqrt{0.5333+0.6613} = \sqrt{1.1946} \approx 1.0930\]

**Critical Value** ($df \approx 59.5$, 90% confidence): $t_c \approx 1.671$

**Confidence Interval:**

\[-2.6 \pm 1.671(1.0930) = -2.6 \pm 1.826\]

\[(-4.426, \ -0.774)\]

**Conclusion:** We are 90% confident that the true difference in average travel time between Route 1 and Route 2 ($\mu_1 - \mu_2$) is between -4.426 and -0.774 minutes. Since the entire interval is below 0, there is evidence that Route 1's average travel time is shorter than Route 2's.

[Return back to Lesson 22.3](https://drolsonmi.github.io/math1040/Lesson22/22_3_ConfidenceIntervals.html#practice)
