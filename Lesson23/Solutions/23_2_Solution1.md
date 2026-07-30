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

1. A marketing team wants to know if customer satisfaction differs between two products. A random sample of 180 Product A customers found 126 satisfied. An independent random sample of 165 Product B customers found 90 satisfied. Build a 95% confidence interval for $p_1 - p_2$.

## Solution

From Lesson 23.1: $\hat{p}_1 = 0.70$ ($n_1 = 180$), $\hat{p}_2 \approx 0.545$ ($n_2 = 165$), conditions verified ✓.

**Point Estimate:**

\[\hat{p}_1 - \hat{p}_2 = 0.70 - 0.545 = 0.155\]

**Standard Error:**

\[SE = \sqrt{\frac{0.70(0.30)}{180}+\frac{0.545(0.455)}{165}} = \sqrt{0.001167+0.001503} = \sqrt{0.002670} \approx 0.0517\]

**Critical Value** (95% confidence, two-tailed): $z_c = 1.960$

**Confidence Interval:**

\[0.155 \pm 1.960(0.0517) = 0.155 \pm 0.1013\]

\[(0.054, \ 0.256)\]

**Conclusion:** We are 95% confident that the true difference in satisfaction rates between Product A and Product B ($p_1 - p_2$) is between 0.054 and 0.256 (5.4 and 25.6 percentage points). Since the entire interval is above 0, there is evidence that Product A has a higher satisfaction rate than Product B.

[Return back to Lesson 23.2](https://drolsonmi.github.io/math1040/Lesson23/23_2_ConfidenceIntervals.html#practice)
