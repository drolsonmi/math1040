<head>
<title>19.2 Practice Problem 2</title>
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
2. A quality control inspector at a factory randomly selects 500 items off the assembly line and finds that 45 are defective. Construct a 99% confidence interval for the true proportion of defective items produced by this factory.

**Step 1: Verify the Central Limit Theorem**

Find the sample proportion and its complement:

$$\hat{p} = \frac{x}{n} = \frac{45}{500} = 0.09 \qquad \hat{q} = 1 - \hat{p} = 0.91$$

* The sample is random — *satisfied*
* $n\hat{p} = 500(0.09) = 45 \ge 10$ — *satisfied*
* $n\hat{q} = 500(0.91) = 455 \ge 10$ — *satisfied*

The Central Limit Theorem applies. We can continue.

**Step 2: Find the Critical Value**

For a 99% confidence level, the remaining 1% is in the tails, with 0.5% in each tail. As we saw in [Lesson 18.1 Critical Values](../../Lesson18/18_1_CriticalValues.md), the critical value for a 99% confidence level is $z_c = \pm 2.58$.

**Step 3: Find the Margin of Error**

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} \\
  &= 2.58\sqrt{\frac{(0.09)(0.91)}{500}} \\
  &= 2.58\sqrt{\frac{0.0819}{500}} \\
  &= 2.58 \times 0.01280 \\
  &\approx 0.033
\end{align*}$$

**Step 4: Find the Confidence Interval**

$$\hat{p} + E = 0.09 + 0.033 = 0.123$$

$$\hat{p} - E = 0.09 - 0.033 = 0.057$$

The confidence interval is $$(0.057,\ 0.123)$$.

**Step 5: Interpret the Confidence Interval**

> **We are 99% confident that the true proportion of defective items produced by this factory is between 0.057 and 0.123 (between 5.7% and 12.3%).**

[Return back to Lesson 19.2](../19_2_ConfidenceIntervalProps.md#practice)