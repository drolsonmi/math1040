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
<title>Solution for practice 6.1.2</title>
</head>

## 6.1 Mean - Solution for Practice 2

2. Consider the dataset \[12, 15, 14, 13, 16, 55\].
  - Find the mean of the dataset as given.
  - Remove the value 55 and find the mean of the remaining five values.
  - Explain what happened to the mean and why.
{:start="2"}

### Solution

**Mean with all six values** ($n = 6$):

$$\bar{x} = \dfrac{12+15+14+13+16+55}{6} = \dfrac{125}{6} \approx 20.83$$

**Mean with the value 55 removed** ($n = 5$):

$$\bar{x} = \dfrac{12+15+14+13+16}{5} = \dfrac{70}{5} = 14$$

**Explanation**: Removing the extreme value of 55 dropped the mean from about 20.83 down to 14 — a difference of nearly 7 points. This happens because the mean is calculated using every value in the dataset, so a single extreme value pulls the mean strongly in its direction. This illustrates why the mean is sensitive to outliers: the more extreme a value is, the more it shifts the mean away from where most of the data actually sits.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson06/6_1_Mean.html#practice)
