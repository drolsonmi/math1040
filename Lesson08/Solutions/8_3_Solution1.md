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
<title>Solution for practice 8.3.1</title>
</head>

## 8.3 Correlation - Solution for Practice 1

1. Recall the practice sets vs. quiz score data from 8.1:

| Practice Sets Completed ($x$) | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| Quiz Score ($y$) | 3 | 5 | 4 | 6 | 7 |

Find the correlation coefficient $r$, and describe the direction and strength of the relationship.

### Solution

We already found most of the needed sums back in 8.1:

$$n = 5, \quad \sum x = 15, \quad \sum y = 25, \quad \sum xy = 84, \quad \sum x^2 = 55$$

We just need one more sum, $\sum y^2$:

| $y$ | $y^2$ |
| --- | --- |
| 3 | 9  |
| 5 | 25 |
| 4 | 16 |
| 6 | 36 |
| 7 | 49 |

$$\sum y^2 = 9+25+16+36+49 = 135$$

**Apply the correlation formula:**

$$r = \frac{n\sum xy - \sum x \sum y}{\sqrt{\left[n\sum x^2 - \left(\sum x\right)^2\right]\left[n\sum y^2 - \left(\sum y\right)^2\right]}}$$

$$r = \frac{5(84) - (15)(25)}{\sqrt{\left[5(55)-(15)^2\right]\left[5(135)-(25)^2\right]}} = \frac{420-375}{\sqrt{(275-225)(675-625)}} = \frac{45}{\sqrt{(50)(50)}} = \frac{45}{50} = 0.9$$

**Interpretation**: $r = 0.9$. Since $r$ is positive, this is a **positive** relationship — as the number of practice sets increases, quiz scores tend to increase as well. Since $|r| = 0.9$ is close to 1, this is a **strong** relationship.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_3_Correlation.html#practice)
