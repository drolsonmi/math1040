<head>
<title>Solution for 5.3.2</title>
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


## 5.3 Histogram Shapes - Solution for Practice 2

2. A real estate agent creates a histogram of home sale prices in a large city. Would you expect this histogram to be symmetric, skewed right, or skewed left? Explain your reasoning.
{:start="2"}

### Solution

We would expect this histogram to be **skewed right**.

Most homes in a city tend to cluster around a typical, moderate price range. However, there is generally no upper limit on how expensive a home can be - a small number of mansions or luxury properties can sell for many times the typical price. These few very expensive homes stretch a long tail out toward the higher values on the right side of the graph, while the bulk of the data (typically priced homes) stays bunched up on the left.

This is a common pattern any time a variable has a natural minimum (a home price can't go below \$0) but no real maximum. Income, home prices, and rent are all classic examples of real-world variables that tend to be skewed right.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson05/5_3_HistogramShapes.html#practice)
