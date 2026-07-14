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
<title>Solution for practice 8.1.2</title>
</head>

## 8.1 Line of Best Fit - Solution for Practice 2

2. A used car dealer records the age of 5 cars (in years) and their resale value (in $1000s):
{:start="2"}

| Age of Car ($x$) | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| Resale Value ($y$) | 20 | 17 | 15 | 12 | 10 |

Find the equation of the line of best fit, $y = a+bx$.

### Solution

**Step 1: Find the needed sums.**

| $x$ | $y$ | $xy$ | $x^2$ |
| --- | --- | --- | --- |
| 1 | 20 | 20  | 1  |
| 2 | 17 | 34  | 4  |
| 3 | 15 | 45  | 9  |
| 4 | 12 | 48  | 16 |
| 5 | 10 | 50  | 25 |

$$n = 5, \quad \sum x = 15, \quad \sum y = 74, \quad \sum xy = 197, \quad \sum x^2 = 55$$

**Step 2: Find the slope, $b$.**

$$b = \frac{n\sum xy - \sum x \sum y}{n\sum x^2 - \left(\sum x\right)^2} = \frac{5(197) - (15)(74)}{5(55) - (15)^2} = \frac{985 - 1110}{275 - 225} = \frac{-125}{50} = -2.5$$

**Step 3: Find the y-intercept, $a$.**

$$\bar{x} = \frac{15}{5} = 3, \qquad \bar{y} = \frac{74}{5} = 14.8$$

$$a = \bar{y} - b\bar{x} = 14.8 - (-2.5)(3) = 14.8 + 7.5 = 22.3$$

**Line of best fit**:

$$y = 22.3 - 2.5x$$

Notice the slope is **negative**, which matches the pattern in the data: as the car's age increases, its resale value decreases.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_1_LineOfBestFit.html#practice)
