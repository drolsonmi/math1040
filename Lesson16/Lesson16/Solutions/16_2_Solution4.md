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
<title>Solution for practice 16.2.4</title>
</head>

## 16.2 Practice Calculating Percentiles/Quartiles - Solution for Practice 4
4. Daily household water usage is approximately normally distributed with $\mu = 300$ gallons and $\sigma = 40$ gallons. Find the **1st quartile ($Q_1$)** of daily water usage.

### Solution

$Q_1$ is the 25th percentile.

**Step 1: Find the z-score with 0.25 area to its left.**

$$P(z<a) = 0.25 \qquad a = ?$$

$$\text{Using a Z-table, } a = -0.675$$

**Step 2: Convert the z-score to a data value.**

$$-0.675 = \frac{x - 300}{40} \qquad\to\qquad x = 300 + 40(-0.675) = 300 - 27 = 273$$

The 1st quartile of daily water usage is about **273 gallons**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson16/16_2_Percentiles.html#practice)
