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
<title>Solution for practice 17.1.3</title>
</head>

## 17.1 Sampling Distributions - Solution for Practice 3
3. A statistics instructor builds two sampling distributions of the average of several dice rolls, using the same number of trials for each. One is built from samples of size 5, and the other from samples of size 40. One histogram is smooth and bell-shaped, and the other is jagged and angular. Which sample size produced the smooth, bell-shaped histogram? Explain your answer.

### Solution

The sample size of **40** produced the smooth, bell-shaped histogram.

As we saw in this lesson, the more dice we average together in a single sample, the more the resulting sampling distribution starts to resemble a normal distribution. With small sample sizes (like $n=5$), there are only a handful of possible average values, so the histogram tends to look angular and blocky. With larger sample sizes (like $n=40$), there are many more possible average values, and the extreme averages become far less likely, pulling the distribution into a smooth, symmetric, bell-shape.

This is the core idea behind the Central Limit Theorem: **as the sample size increases, the sampling distribution of the mean becomes more and more normal**, regardless of the shape of the original population distribution.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_1_SamplingDistributions.html#practice)
