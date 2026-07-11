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
<title>Solution for practice 8.1.3</title>
</head>

## 8.1 Line of Best Fit - Solution for Practice 3

1. A researcher records the outdoor temperature (in °F) and a shop's ice cream sales (in $100s) on 5 different days:

| Temperature ($x$) | 60 | 70 | 80 | 90 | 100 |
| --- | --- | --- | --- | --- | --- |
| Ice Cream Sales ($y$) | 2 | 4 | 5 | 7 | 9 |

Find the equation of the line of best fit, $y=a+bx$, and interpret the slope in the context of the problem. Does the y-intercept have a meaningful real-world interpretation here? Explain.

### Solution

**Step 1: Find the needed sums.**

| $x$ | $y$ | $xy$ | $x^2$ |
| --- | --- | --- | --- |
| 60  | 2 | 120 | 3600  |
| 70  | 4 | 280 | 4900  |
| 80  | 5 | 400 | 6400  |
| 90  | 7 | 630 | 8100  |
| 100 | 9 | 900 | 10000 |

$$n = 5, \quad \sum x = 400, \quad \sum y = 27, \quad \sum xy = 2330, \quad \sum x^2 = 33000$$

**Step 2: Find the slope, $b$.**

$$b = \frac{n\sum xy - \sum x \sum y}{n\sum x^2 - \left(\sum x\right)^2} = \frac{5(2330) - (400)(27)}{5(33000) - (400)^2} = \frac{11650 - 10800}{165000 - 160000} = \frac{850}{5000} = 0.17$$

**Step 3: Find the y-intercept, $a$.**

$$\bar{x} = \frac{400}{5} = 80, \qquad \bar{y} = \frac{27}{5} = 5.4$$

$$a = \bar{y} - b\bar{x} = 5.4 - (0.17)(80) = 5.4 - 13.6 = -8.2$$

**Line of best fit**:

$$y = -8.2 + 0.17x$$

**Interpreting the slope**: The slope, $b = 0.17$, means that for every 1°F increase in temperature, ice cream sales increase by about 0.17 hundred dollars — roughly **$17**.

**Interpreting the y-intercept**: The y-intercept, $a = -8.2$, would represent the predicted sales when the temperature is 0°F. This value is **not meaningful** in context, for two reasons: sales of $-820$ (negative sales) doesn't make real-world sense, and 0°F is far **outside the range of the original data** (60°F to 100°F). Using the line to predict at $x=0$ would be an example of **extrapolation** — assuming the linear pattern continues far beyond where we actually have data, which is not a safe assumption here. The y-intercept in this case is simply a mathematical byproduct of the line's equation, not a value we should trust or interpret.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_1_LineOfBestFit.html#practice)
