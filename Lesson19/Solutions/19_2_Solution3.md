<head>
<title>19.2 Practice Problem 3</title>
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
3. A university researcher surveys a random sample of 180 students and finds that 63 report experiencing high levels of stress during finals week. Construct a 90% confidence interval for the true proportion of students who experience high stress during finals week.

**Step 1: Verify the Central Limit Theorem**

Find the sample proportion and its complement:

$$\hat{p} = \frac{x}{n} = \frac{63}{180} = 0.35 \qquad \hat{q} = 1 - \hat{p} = 0.65$$

* The sample is random — *satisfied*
* $n\hat{p} = 180(0.35) = 63 \ge 10$ — *satisfied*
* $n\hat{q} = 180(0.65) = 117 \ge 10$ — *satisfied*

The Central Limit Theorem applies. We can continue.

**Step 2: Find the Critical Value**

For a 90% confidence level, the remaining 10% is in the tails, with 5% in each tail. As we saw in [Lesson 18.1 Critical Values](../../Lesson18/18_1_CriticalValues.md), the critical value for a 90% confidence level is $z_c = \pm 1.645$.

**Step 3: Find the Margin of Error**

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} \\
  &= 1.645\sqrt{\frac{(0.35)(0.65)}{180}} \\
  &= 1.645\sqrt{\frac{0.2275}{180}} \\
  &= 1.645 \times 0.03555 \\
  &\approx 0.058
\end{align*}$$

**Step 4: Find the Confidence Interval**

$$\hat{p} + E = 0.35 + 0.058 = 0.408$$

$$\hat{p} - E = 0.35 - 0.058 = 0.292$$

The confidence interval is $$(0.292,\ 0.408)$$.

**Step 5: Interpret the Confidence Interval**

> **We are 90% confident that the true proportion of students who experience high levels of stress during finals week is between 0.292 and 0.408 (between 29.2% and 40.8%).**

[Return back to Lesson 19.2](../19_2_ConfidenceIntervalProps.md#practice)