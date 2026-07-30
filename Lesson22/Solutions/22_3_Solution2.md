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

1. A fitness researcher wants to know if Program X leads to greater average weight loss than Program Y. A random sample of 25 participants using Program X lost an average of 12.3 lbs with a standard deviation of 3.1 lbs. An independent random sample of 28 participants using Program Y lost an average of 9.8 lbs with a standard deviation of 2.8 lbs. Build a 98% confidence interval for $\mu_1 - \mu_2$ (use $df \approx 49.8$).

## Solution

From Lesson 22.2 we have:

- $n_1 = 25$, $\bar{x}_1 = 12.3$, $s_1 = 3.1$
- $n_2 = 28$, $\bar{x}_2 = 9.8$, $s_2 = 2.8$
- Conditions verified ✓

Since this is ultimately headed toward a right-tailed test at $\alpha = 0.01$, we use a two-sided confidence level of $1-2\alpha = 0.98$, or 98%.

**Point Estimate:**

\[\bar{x}_1 - \bar{x}_2 = 12.3 - 9.8 = 2.5\]

**Standard Error:**

\[SE = \sqrt{\frac{3.1^2}{25}+\frac{2.8^2}{28}} = \sqrt{0.3844+0.28} = \sqrt{0.6644} \approx 0.8151\]

**Critical Value** ($df \approx 49.8$, 98% confidence): $t_c \approx 2.403$

**Confidence Interval:**

\[2.5 \pm 2.403(0.8151) = 2.5 \pm 1.959\]

\[(0.541, \ 4.459)\]

**Conclusion:** We are 98% confident that the true difference in average weight loss between Program X and Program Y ($\mu_1 - \mu_2$) is between 0.541 and 4.459 lbs. Since the entire interval is above 0, there is evidence that Program X leads to greater average weight loss than Program Y.

[Return back to Lesson 22.3](https://drolsonmi.github.io/math1040/Lesson22/22_3_ConfidenceIntervals.html#practice)
