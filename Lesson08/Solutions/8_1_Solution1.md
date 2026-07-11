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
<title>Solution for practice 8.1.1</title>
</head>

## 8.1 Line of Best Fit - Solution for Practice 1

1. A tutor records the number of practice problem sets a student completes and the student's score (out of 10) on the following quiz:

| Practice Sets Completed ($x$) | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| Quiz Score ($y$) | 3 | 5 | 4 | 6 | 7 |

Find the equation of the line of best fit, $y = a+bx$.

### Solution

In practice, you'll find $a$ and $b$ using technology (see the Technology section on the lesson page). This solution also shows the underlying calculation so you can see where those numbers come from.

**Step 1: Find the needed sums.**

| $x$ | $y$ | $xy$ | $x^2$ |
| --- | --- | --- | --- |
| 1 | 3 | 3  | 1  |
| 2 | 5 | 10 | 4  |
| 3 | 4 | 12 | 9  |
| 4 | 6 | 24 | 16 |
| 5 | 7 | 35 | 25 |

$$n = 5, \quad \sum x = 15, \quad \sum y = 25, \quad \sum xy = 84, \quad \sum x^2 = 55$$

**Step 2: Find the slope, $b$.**

$$b = \frac{n\sum xy - \sum x \sum y}{n\sum x^2 - \left(\sum x\right)^2} = \frac{5(84) - (15)(25)}{5(55) - (15)^2} = \frac{420 - 375}{275 - 225} = \frac{45}{50} = 0.9$$

**Step 3: Find the y-intercept, $a$.**

$$\bar{x} = \frac{15}{5} = 3, \qquad \bar{y} = \frac{25}{5} = 5$$

$$a = \bar{y} - b\bar{x} = 5 - (0.9)(3) = 5 - 2.7 = 2.3$$

**Line of best fit**:

$$y = 2.3 + 0.9x$$

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_1_LineOfBestFit.html#practice)
