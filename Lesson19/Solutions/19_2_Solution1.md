<head>
<title>19.2 Practice Problem 1</title>
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
1. A local news station surveys a random sample of 300 residents and finds that 174 support a proposed new park. Construct a 95% confidence interval for the true proportion of residents who support the new park.

**Step 1: Verify the Central Limit Theorem**

Find the sample proportion and its complement:

$$\hat{p} = \frac{x}{n} = \frac{174}{300} = 0.58 \qquad \hat{q} = 1 - \hat{p} = 0.42$$

* The sample is random — *satisfied*
* $$n\hat{p} = 300(0.58) = 174 \ge 10$$ — *satisfied*
* $$n\hat{q} = 300(0.42) = 126 \ge 10$$ — *satisfied*

The Central Limit Theorem applies. We can continue.

**Step 2: Find the Critical Value**

For a 95% confidence level, the remaining 5% is in the tails, with 2.5% in each tail. Using a Z-Table with a left tail area of 2.5%:

<img src="../images/Fig19_2a_Practice1_ZTable.png?raw=true" width="500" alt="95% Confidence Level on a Z-Table">

The critical value is $$z_c = \pm 1.96$$.

**Step 3: Find the Margin of Error**

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} \\
  &= 1.96\sqrt{\frac{(0.58)(0.42)}{300}} \\
  &= 1.96\sqrt{\frac{0.2436}{300}} \\
  &= 1.96 \times 0.02850 \\
  &\approx 0.056
\end{align*}$$

**Step 4: Find the Confidence Interval**

$$\hat{p} + E = 0.58 + 0.056 = 0.636$$

$$\hat{p} - E = 0.58 - 0.056 = 0.524$$

The confidence interval is $$(0.524,\ 0.636)$$.

**Step 5: Interpret the Confidence Interval**

> **We are 95% confident that the true proportion of residents who support the proposed new park is between 0.524 and 0.636 (between 52.4% and 63.6%).**

We can verify this result using Desmos:

<img src="../images/Fig19_2a_Practice1_Desmos.png?raw=true" width="500" alt="95% Confidence Interval for a Proportion on Desmos">

[Return back to Lesson 19.2](../19_2_ConfidenceInterval_Proportion.md#practice)