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

1. An education researcher wants to know if there is a difference in average test scores between School A and School B. A random sample of 40 students at School A had an average score of 78.4 with a standard deviation of 8.2. An independent random sample of 38 students at School B had an average score of 74.9 with a standard deviation of 7.5. Build a 95% confidence interval for $\mu_1 - \mu_2$ (use $df \approx 75.7$).

## Solution

From Lesson 22.2 we have:

- $n_1 = 40$, $\bar{x}_1 = 78.4$, $s_1 = 8.2$
- $n_2 = 38$, $\bar{x}_2 = 74.9$, $s_2 = 7.5$
- Conditions verified ✓

**Point Estimate:**

\[\bar{x}_1 - \bar{x}_2 = 78.4 - 74.9 = 3.5\]

**Standard Error:**

\[SE = \sqrt{\frac{8.2^2}{40}+\frac{7.5^2}{38}} = \sqrt{1.681+1.480} = \sqrt{3.161} \approx 1.778\]

**Critical Value** ($df \approx 75.7$, 95% confidence): $t_c \approx 1.992$

**Confidence Interval:**

\[3.5 \pm 1.992(1.778) = 3.5 \pm 3.542\]

\[(-0.042, \ 7.042)\]

**Conclusion:** We are 95% confident that the true difference in average test scores between School A and School B ($\mu_1 - \mu_2$) is between -0.042 and 7.042 points. Since the interval **contains 0**, we don't have enough evidence to conclude that the two schools' average test scores are different.

[Return back to Lesson 22.3](https://drolsonmi.github.io/math1040/Lesson22/22_3_ConfidenceIntervals.html#practice)
