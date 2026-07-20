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
<title>Solution for practice 16.2.2</title>
</head>

## 16.2 Practice Calculating Percentiles/Quartiles - Solution for Practice 2
2. SAT Math scores are approximately normally distributed with $\mu = 520$ and $\sigma = 100$. Find the minimum score needed for the top 10% of scorers, i.e. the **90th percentile**.

### Solution

**Step 1: Find the z-score with 0.90 area to its left.**

$$P(z<a) = 0.90 \qquad a = ?$$

$$\text{Using a Z-table, } a \approx 1.28$$

**Step 2: Convert the z-score to a data value.**

$$1.28 = \frac{x - 520}{100} \qquad\to\qquad x = 520 + 100(1.28) = 520 + 128 = 648$$

A score of about **648** is needed to be in the top 10% of scorers.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson16/16_2_Percentiles.html#practice)
