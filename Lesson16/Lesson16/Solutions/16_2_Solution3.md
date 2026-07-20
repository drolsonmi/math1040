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
<title>Solution for practice 16.2.3</title>
</head>

## 16.2 Practice Calculating Percentiles/Quartiles - Solution for Practice 3
3. Phone battery life is approximately normally distributed with $\mu = 11$ hours and $\sigma = 1.2$ hours. Find the **3rd quartile ($Q_3$)** of battery life.

### Solution

$Q_3$ is the 75th percentile.

**Step 1: Find the z-score with 0.75 area to its left.**

$$P(z<a) = 0.75 \qquad a = ?$$

$$\text{Using a Z-table, } a = 0.675$$

**Step 2: Convert the z-score to a data value.**

$$0.675 = \frac{x - 11}{1.2} \qquad\to\qquad x = 11 + 1.2(0.675) = 11 + 0.81 = 11.81$$

The 3rd quartile of battery life is about **11.81 hours**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson16/16_2_Percentiles.html#practice)
