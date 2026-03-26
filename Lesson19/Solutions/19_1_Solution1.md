<head>
<title>19.1 Practice Problem 1</title>
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
1. A poll asks whether registered voters plan to vote in the upcoming election. In a random sample of 150 voters, 96 say they plan to vote. Find the margin of error at the 90% confidence level.

First, find the sample proportion and its complement:

$$\hat{p} = \frac{x}{n} = \frac{96}{150} = 0.64 \qquad \hat{q} = 1 - \hat{p} = 0.36$$

Verify the Central Limit Theorem applies:
* The sample is random — *satisfied*
* $$n\hat{p} = 150(0.64) = 96 \ge 10$$ — *satisfied*
* $$n\hat{q} = 150(0.36) = 54 \ge 10$$ — *satisfied*

Find the critical value. For a 90% confidence level, the remaining 10% is in the tails, with 5% in each tail. Using a Z-Table with a left tail area of 5%:

<img src="../images/Fig19_1a_Practice1_ZTable.png?raw=true" width="500" alt="90% Confidence Level on a Z-Table">

The critical value is $$z_c = \pm 1.645$$.

Now calculate the margin of error:

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} \\
  &= 1.645\sqrt{\frac{(0.64)(0.36)}{150}} \\
  &= 1.645\sqrt{\frac{0.2304}{150}} \\
  &= 1.645 \times 0.03919 \\
  &\approx \mathbf{0.064}
\end{align*}$$

The margin of error is **0.064**, or about **6.4 percentage points**.

We can verify this result using Desmos by computing the margin of error formula directly:

<img src="../images/Fig19_1a_Practice1_Desmos.png?raw=true" width="500" alt="90% Confidence Level Margin of Error on Desmos">

[Return back to Lesson 19.1](../19_1_CriticalValue_MarginOfError.md#practice)