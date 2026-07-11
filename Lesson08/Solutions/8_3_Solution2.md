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
<title>Solution for practice 8.3.2</title>
</head>

## 8.3 Correlation - Solution for Practice 2

1. Recall the car age vs. resale value data from 8.1:

| Age of Car ($x$) | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| Resale Value ($y$) | 20 | 17 | 15 | 12 | 10 |

Find the correlation coefficient $r$, and describe the direction and strength of the relationship.

### Solution

We already found most of the needed sums back in 8.1:

$$n = 5, \quad \sum x = 15, \quad \sum y = 74, \quad \sum xy = 197, \quad \sum x^2 = 55$$

We just need one more sum, $\sum y^2$:

| $y$ | $y^2$ |
| --- | --- |
| 20 | 400 |
| 17 | 289 |
| 15 | 225 |
| 12 | 144 |
| 10 | 100 |

$$\sum y^2 = 400+289+225+144+100 = 1158$$

**Apply the correlation formula:**

$$r = \frac{n\sum xy - \sum x \sum y}{\sqrt{\left[n\sum x^2 - \left(\sum x\right)^2\right]\left[n\sum y^2 - \left(\sum y\right)^2\right]}}$$

$$r = \frac{5(197) - (15)(74)}{\sqrt{\left[5(55)-(15)^2\right]\left[5(1158)-(74)^2\right]}} = \frac{985-1110}{\sqrt{(275-225)(5790-5476)}} = \frac{-125}{\sqrt{(50)(314)}} = \frac{-125}{\sqrt{15700}} \approx \frac{-125}{125.30} \approx -0.998$$

**Interpretation**: $r \approx -0.998$. Since $r$ is negative, this is a **negative** relationship — as a car's age increases, its resale value tends to decrease. Since $|r| \approx 0.998$ is extremely close to 1, this is a **very strong** relationship — the data points fall almost exactly on a straight line.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_3_Correlation.html#practice)
