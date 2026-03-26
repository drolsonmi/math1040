<head>
<title>19.1 Practice Problem 3</title>
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
3. A health survey of 250 randomly selected adults finds that 85 report exercising at least 3 times per week. Find the margin of error at the 99% confidence level.

First, find the sample proportion and its complement:

$$\hat{p} = \frac{x}{n} = \frac{85}{250} = 0.34 \qquad \hat{q} = 1 - \hat{p} = 0.66$$

Verify the Central Limit Theorem applies:
* The sample is random — *satisfied*
* $n\hat{p} = 250(0.34) = 85 \ge 10$ — *satisfied*
* $n\hat{q} = 250(0.66) = 165 \ge 10$ — *satisfied*

Find the critical value. For a 99% confidence level, the remaining 1% is in the tails, with 0.5% in each tail. As we saw in [Lesson 18.1 Critical Values](../../Lesson18/18_1_CriticalValues.md), the critical value for a 99% confidence level is $z_c = \pm 2.58$.

Now calculate the margin of error:

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} \\
  &= 2.58\sqrt{\frac{(0.34)(0.66)}{250}} \\
  &= 2.58\sqrt{\frac{0.2244}{250}} \\
  &= 2.58 \times 0.02996 \\
  &\approx \mathbf{0.077}
\end{align*}$$

The margin of error is **0.077**, or about **7.7 percentage points**.

[Return back to Lesson 19.1](../19_1_CriticalValues.md#practice)