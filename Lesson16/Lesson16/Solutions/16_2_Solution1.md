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
<title>Solution for practice 16.2.1</title>
</head>

## 16.2 Practice Calculating Percentiles/Quartiles - Solution for Practice 1
1. Human pregnancy length is approximately normally distributed with $\mu = 268$ days and $\sigma = 15$ days. Find the length that marks the **10th percentile**.

### Solution

**Step 1: Find the z-score with 0.10 area to its left.**

$$P(z<a) = 0.10 \qquad a = ?$$

$$\text{Using a Z-table, } a \approx -1.28$$

**Step 2: Convert the z-score to a data value.**

$$-1.28 = \frac{x - 268}{15} \qquad\to\qquad x = 268 + 15(-1.28) = 268 - 19.2 = 248.8$$

A pregnancy length of about **248.8 days** marks the 10th percentile.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson16/16_2_Percentiles.html#practice)
