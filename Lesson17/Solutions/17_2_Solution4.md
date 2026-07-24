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
<title>Solution for practice 17.2.4</title>
</head>

## 17.2 Statistics of Sampling Distributions - Solution for Practice 4
4. SAT scores for a particular year have a population mean of $\mu = 1050$ and a standard deviation of $\sigma = 200$.
    - Find $\sigma_{\bar{x}}$ for random samples of size $n = 25$.
    - Find $\sigma_{\bar{x}}$ for random samples of size $n = 100$.
    - Compare your two answers.

### Solution

**Samples of size $n = 25$:**

$$\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{200}{\sqrt{25}} = \frac{200}{5} = 40$$

**Samples of size $n = 100$:**

$$\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{200}{\sqrt{100}} = \frac{200}{10} = 20$$

**Comparison:**

Quadrupling the sample size from 25 to 100 cut the standard deviation of the sampling distribution in half, from 40 down to 20. This shows the general relationship between sample size and spread: **as the sample size increases, $\sigma_{\bar{x}}$ decreases**, meaning the sample means cluster more tightly around the population mean. Larger samples give us more precise (less variable) estimates of the population mean - though because of the square root in the formula, we have to *quadruple* the sample size to cut the standard deviation in half, not just double it.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_2_StatsOfSamplingDists.html#practice)
