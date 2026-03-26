<head>
<title>19.1 Practice Problem 2</title>
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
2. A random sample of 400 households in a city finds that 112 own a pet. Find the margin of error at the 95% confidence level.

First, find the sample proportion and its complement:

$$\hat{p} = \frac{x}{n} = \frac{112}{400} = 0.28 \qquad \hat{q} = 1 - \hat{p} = 0.72$$

Verify the Central Limit Theorem applies:
* The sample is random — *satisfied*
* $n\hat{p} = 400(0.28) = 112 \ge 10$ — *satisfied*
* $n\hat{q} = 400(0.72) = 288 \ge 10$ — *satisfied*

Find the critical value. For a 95% confidence level, the remaining 5% is in the tails, with 2.5% in each tail. As we saw in [Lesson 18.1 Critical Values](../../Lesson18/18_1_CriticalValues.md), the critical value for a 95% confidence level is $z_c = \pm 1.96$.

Now calculate the margin of error:

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} \\
  &= 1.96\sqrt{\frac{(0.28)(0.72)}{400}} \\
  &= 1.96\sqrt{\frac{0.2016}{400}} \\
  &= 1.96 \times 0.02245 \\
  &\approx \mathbf{0.044}
\end{align*}$$

The margin of error is **0.044**, or about **4.4 percentage points**.

[Return back to Lesson 19.1](../19_1_CriticalValues.md#practice)