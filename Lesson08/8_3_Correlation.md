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
</head>

# Lesson 8.3 Correlation
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 8.1.4 Describing linear relationships with correlation (pages 346-348)

## Lesson
In 8.1, we fit a line directly through our data. But how do we know whether that line is actually a *good* fit? The **correlation coefficient**, denoted $r$, gives us a single number that measures how strong a linear relationship is between two quantitative variables, and in which direction it goes.
 
### The Formula
 
$$r = \frac{n\sum xy - \sum x \sum y}{\sqrt{\left[n\sum x^2 - \left(\sum x\right)^2\right]\left[n\sum y^2 - \left(\sum y\right)^2\right]}}$$
 
In practice, you'll almost always calculate $r$ using technology rather than by hand (see the Technology section below) — but it's worth knowing that $r$ is built from the same sums we already used to find the line of best fit.
 
### Interpreting $r$
 
No matter how many data points you have, $r$ will always fall somewhere between $-1$ and $1$:
 
$$-1 \le r \le 1$$
 
- The **sign** of $r$ tells you the **direction** of the relationship:
  - $r > 0$: a **positive** relationship (as $x$ increases, $y$ tends to increase)
  - $r < 0$: a **negative** relationship (as $x$ increases, $y$ tends to decrease)
- The **size** of $r$ (how close it is to $-1$ or $1$) tells you the **strength** of the relationship:
  - $r$ close to $\pm1$: a **strong** linear relationship — the data points sit close to a straight line
  - $r$ close to $0$: a **weak** (or no) linear relationship — the data points are scattered with little to no linear pattern
  - $r = 0$: no linear relationship at all
A common rough guideline used to describe the strength of $r$:
 
| $|r|$ | Strength |
| --- | --- |
| 0.00 - 0.29 | weak |
| 0.30 - 0.69 | moderate |
| 0.70 - 1.00 | strong |
 
### A Few Important Cautions
 
- **Correlation measures only *linear* relationships.** Two variables can have a strong, obvious pattern (like a curve) and still produce a correlation coefficient close to 0, simply because that pattern isn't a straight line. Always look at the scatterplot, not just the value of $r$.
- **Correlation is not causation.** Just like we discussed back in Lesson 4, a strong correlation between two variables doesn't mean one *causes* the other. There could be a lurking variable responsible for both, or the relationship could be coincidental.
- **Correlation is sensitive to outliers.** A single unusual data point can noticeably strengthen or weaken the value of $r$, especially in a small dataset.

<iframe width="560" height="315" src="https://www.youtube.com/embed/V8hAoJfP_vA?si=-XL0dAOYGmXw2hOd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. Recall the practice sets vs. quiz score data from 8.1:
| Practice Sets Completed ($x$) | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| Quiz Score ($y$) | 3 | 5 | 4 | 6 | 7 |
 
  Find the correlation coefficient $r$, and describe the direction and strength of the relationship.
  - [After solving on your own, see solution here](./Solutions/8_3_Solution1.html)
2. Recall the car age vs. resale value data from 8.1:
| Age of Car ($x$) | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| Resale Value ($y$) | 20 | 17 | 15 | 12 | 10 |
 
  Find the correlation coefficient $r$, and describe the direction and strength of the relationship.
  - [After solving on your own, see solution here](./Solutions/8_3_Solution2.html)
3. For each correlation coefficient below, describe the direction (positive or negative) and strength (weak, moderate, or strong) of the relationship:
  - $r = 0.85$
  - $r = -0.42$
  - $r = 0.05$
  - $r = -0.95$
  - [After solving on your own, see solution here](./Solutions/8_3_Solution3.html)


## Technology

### TI-83/84
The correlation coefficient $r$ is calculated at the same time as the line of best fit, but you may need to turn on Diagnostics first before $r$ will show up.
 
1. Turn on Diagnostics (only needs to be done once):
    - Press **2nd**,
    - Press **0** (CATALOG)
    - Scroll down to **DiagnosticOn**
    - Press **ENTER** twice
2. Press **STAT**, then select **1: Edit**, and enter your $x$-values into **L1** and your $y$-values into **L2**.
3. Press **STAT**, arrow over to **CALC**, and select **4: LinReg(ax+b)**.
4. Set **Xlist** to **L1** and **Ylist** to **L2**, then select **Calculate** and press **ENTER**.
5. Scroll down through the output. Along with $a$ and $b$, you'll now also see:
  - **$r$** — the correlation coefficient
  - **$r^2$** — the coefficient of determination

<iframe width="560" height="315" src="https://www.youtube.com/embed/40bG6YErzGA?si=OXEAR5CZAPFfleFU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


### Excel
1. Enter your $x$-values in one column (for example, column A) and your $y$-values in the adjacent column (column B).
2. Click on an empty cell and enter:
   `=CORREL(A1:A10, B1:B10)`
   (Adjust the cell range to match wherever your data is located. It doesn't matter which column you list first.)
3. This returns the correlation coefficient $r$ directly.
4. If you added a trendline to a scatterplot (see 8.1), checking **Display R-squared value on chart** will show you $r^2$ — just take the square root (and match the sign of the slope) to get $r$.


### Desmos 
1. Go to [desmos.com/calculator](https://www.desmos.com/calculator).
2. Enter your data into a table, with $x$-values in the first column and $y$-values in the second column (see 8.1 for details).
3. On a new line, run the regression: `y1 ~ a*x1 + b`
4. Once the regression runs, click on the small gray box to the left of the regression line to expand the statistics. Desmos will display $r^2$ directly beneath the regression equation.

This video was shown in [8.1](8_1_LineOfBestFit.md) on the Line of Best Fit. It is good to watch again, but if you are shaky with line of best fit, go ahead and watch it again. You'll see the correlation in the calculation as I mention in the video.

<iframe width="560" height="315" src="https://www.youtube.com/embed/tdikTkheCfs?si=BVpObVSk4ApqxVMw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

The correlation according to Desmos is *r = 0.9233*. This indicates a __high positive__ correlation. That means that there is a __strong__ relationship and the relationship is __positive__ (as one variable increases, the other increases as well).