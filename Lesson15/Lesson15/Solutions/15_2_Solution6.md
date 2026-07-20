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
<title>Solution for practice 15.2.6</title>
</head>

## 15.2 The Normal Distribution - Solution for Practice 6
6. Using the height distribution ($\mu = 69$ in, $\sigma = 2.8$ in), estimate the percentage of men **taller than 74.6 inches**.

### Solution

First, notice that $74.6 = 69 + 2(2.8)$, so 74.6 inches is exactly 2 standard deviations above the mean ($z = 2$). By the Empirical Rule, 95% of values fall within 2 standard deviations of the mean, leaving $100\% - 95\% = 5\%$ split evenly between the two tails:

$$\frac{100\%-95\%}{2}=\frac{5\%}{2}=2.5\%$$

About **2.5%** of men are taller than 74.6 inches.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson15/15_2_NormalDistributions.html#practice)
