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
<title>Solution for practice 17.2.2</title>
</head>

## 17.2 Statistics of Sampling Distributions - Solution for Practice 2
2. Human body temperature has a population mean of $\mu = 98.6\degree F$ and a standard deviation of $\sigma = 0.7\degree F$. A nurse records the average temperature of a random sample of 49 patients. Find $\mu_{\bar{x}}$ and $\sigma_{\bar{x}}$, and explain what $\sigma_{\bar{x}}$ tells you in this context.

### Solution

**Sampling mean:**

$$\mu_{\bar{x}} = \mu = 98.6\degree F$$

**Sampling standard deviation:**

$$\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{0.7}{\sqrt{49}} = \frac{0.7}{7} = 0.1\degree F$$

**Interpretation:**

$\sigma_{\bar{x}} = 0.1\degree F$ tells us how much the average temperature of a random sample of 49 patients typically varies from the true population mean of $98.6\degree F$. Notice how much smaller this is than the standard deviation of a single patient's temperature ($\sigma = 0.7\degree F$) - averaging over 49 patients gives a much more precise estimate of the population mean than a single measurement would.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_2_StatsOfSamplingDists.html#practice)
