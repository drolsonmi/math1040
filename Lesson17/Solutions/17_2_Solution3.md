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
<title>Solution for practice 17.2.3</title>
</head>

## 17.2 Statistics of Sampling Distributions - Solution for Practice 3
3. A machine fills water bottles, and the amount it dispenses has some unknown population standard deviation $\sigma$. A quality control team takes repeated samples of size $n = 36$ bottles, and finds that the resulting sampling distribution has a standard deviation of $\sigma_{\bar{x}} = 3$ mL. What is the population standard deviation $\sigma$?

### Solution

This problem gives us $\sigma_{\bar{x}}$ and $n$, and asks us to work backwards to find $\sigma$. Let's start with the formula and solve it for $\sigma$.

$$\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$$

**Step 1: Multiply both sides by $\sqrt{n}$.**

$$\sigma = \sigma_{\bar{x}} \cdot \sqrt{n}$$

**Step 2: Substitute in the known values.**

$$\sigma = 3 \cdot \sqrt{36} = 3 \cdot 6 = 18$$

The population standard deviation is $\sigma = 18$ mL.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_2_StatsOfSamplingDists.html#practice)
