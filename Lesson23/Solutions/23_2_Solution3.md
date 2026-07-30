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

1. A quality control manager wants to know if Machine A has a lower defect rate than Machine B. A random sample of 200 items from Machine A found 14 defective. An independent random sample of 220 items from Machine B found 24 defective. Build a 90% confidence interval for $p_1 - p_2$.

## Solution

From Lesson 23.1: $\hat{p}_1 = 0.07$ ($n_1 = 200$), $\hat{p}_2 \approx 0.109$ ($n_2 = 220$), conditions verified ✓.

Since this is ultimately headed toward a left-tailed test at $\alpha = 0.05$, we use a two-sided confidence level of $1-2\alpha = 0.90$, or 90%.

**Point Estimate:**

\[\hat{p}_1 - \hat{p}_2 = 0.07 - 0.109 = -0.039\]

**Standard Error:**

\[SE = \sqrt{\frac{0.07(0.93)}{200}+\frac{0.109(0.891)}{220}} = \sqrt{0.0003255+0.0004415} = \sqrt{0.0007670} \approx 0.0277\]

**Critical Value** (90% confidence, two-tailed): $z_c = 1.645$

**Confidence Interval:**

\[-0.039 \pm 1.645(0.0277) = -0.039 \pm 0.0456\]

\[(-0.085, \ 0.007)\]

**Conclusion:** We are 90% confident that the true difference in defect rates between Machine A and Machine B ($p_1 - p_2$) is between -0.085 and 0.007 (-8.5 and 0.7 percentage points). Since the interval **contains 0**, we don't have enough evidence to say Machine A's defect rate is lower than Machine B's.

[Return back to Lesson 23.2](https://drolsonmi.github.io/math1040/Lesson23/23_2_ConfidenceIntervals.html#practice)
