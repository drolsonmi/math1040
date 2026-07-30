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

1. A public health department wants to know if a new smoking cessation program has a higher success rate than the standard program. A random sample of 140 participants in the new program found that 42 successfully quit smoking. An independent random sample of 150 participants in the standard program found that 27 successfully quit. Build a 98% confidence interval for $p_1 - p_2$.

## Solution

From Lesson 23.1: $\hat{p}_1 = 0.30$ ($n_1 = 140$), $\hat{p}_2 = 0.18$ ($n_2 = 150$), conditions verified ✓.

Since this is ultimately headed toward a right-tailed test at $\alpha = 0.01$, we use a two-sided confidence level of $1-2\alpha = 0.98$, or 98%.

**Point Estimate:**

\[\hat{p}_1 - \hat{p}_2 = 0.30 - 0.18 = 0.12\]

**Standard Error:**

\[SE = \sqrt{\frac{0.30(0.70)}{140}+\frac{0.18(0.82)}{150}} = \sqrt{0.0015+0.000984} = \sqrt{0.002484} \approx 0.0498\]

**Critical Value** (98% confidence, two-tailed): $z_c = 2.326$

**Confidence Interval:**

\[0.12 \pm 2.326(0.0498) = 0.12 \pm 0.1159\]

\[(0.004, \ 0.236)\]

**Conclusion:** We are 98% confident that the true difference in success rates between the new and standard programs ($p_1 - p_2$) is between 0.004 and 0.236 (0.4 and 23.6 percentage points). Since the entire interval is above 0, there is evidence that the new program has a higher success rate than the standard program.

[Return back to Lesson 23.2](https://drolsonmi.github.io/math1040/Lesson23/23_2_ConfidenceIntervals.html#practice)
