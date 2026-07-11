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

# Lesson 8.4 The Coefficient of Determination
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 8.2.6 Using $$r^2$$ to describe the strength of a fit (pages 354-355)

## Lesson
We just learned that the correlation coefficient $r$ tells us the direction and strength of a linear relationship. The **coefficient of determination**, $r^2$, builds on this by telling us something even more concrete: **the percentage of the variation in $y$ that is explained by its linear relationship with $x$.**
 
### The Formula
 
The coefficient of determination is simply the square of the correlation coefficient:
 
$$r^2$$
 
Since $r$ is always between $-1$ and $1$, squaring it means $r^2$ is always between $0$ and $1$:
 
$$0 \le r^2 \le 1$$
 
Unlike $r$, the coefficient of determination is **never negative** — it doesn't tell us the *direction* of the relationship, only how much of the variation is explained by it.
 
### Interpreting $r^2$
 
We usually express $r^2$ as a percentage. For example, if $r^2 = 0.81$, we would say:
 
> "About 81% of the variation in $y$ can be explained by the linear relationship with $x$."
 
This also means the remaining $100\% - 81\% = 19\%$ of the variation in $y$ is due to **other factors** — things not captured by $x$ alone, such as other variables we haven't measured, or natural randomness.
 
- An $r^2$ **close to 1** means the line of best fit explains most of the variation in the data — the data points sit close to the line, and $x$ is a strong predictor of $y$.
- An $r^2$ **close to 0** means the line of best fit explains very little of the variation in the data — knowing $x$ doesn't tell you much about what $y$ will be.

### Why Use $r^2$ Instead of Just $r$?
 
While $r$ is useful for quickly checking the direction and general strength of a relationship, $r^2$ gives us a more intuitive, real-world interpretation: a *percentage* of variation explained. This makes it easier to communicate just how useful a linear model actually is. It's also worth noticing that a relatively modest-looking correlation can translate into a much smaller coefficient of determination — for example, $r = 0.5$ might sound like a moderate relationship, but $r^2 = 0.25$ means the line only explains 25% of the variation in the data, leaving 75% unexplained.

<iframe width="560" height="315" src="https://www.youtube.com/embed/2zr785gdILA?si=Uzs_MigIiUpdsQxi" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. In 8.3, we found that the correlation coefficient for the practice sets vs. quiz score data was $r = 0.9$. Find the coefficient of determination, $r^2$, and interpret it in the context of this problem.
  - [After solving on your own, see solution here](./Solutions/8_4_Solution1.html)
2. In 8.3, we found that the correlation coefficient for the car age vs. resale value data was $r \approx -0.998$. Find the coefficient of determination, $r^2$, and interpret it in the context of this problem.
  - [After solving on your own, see solution here](./Solutions/8_4_Solution2.html)
3. A dataset has a coefficient of determination of $r^2 = 0.36$.
  - What percentage of the variation in $y$ is explained by the linear relationship with $x$?
  - What are the two possible values of the correlation coefficient $r$?
  - Can you tell from $r^2$ alone whether the relationship is positive or negative? Explain.
  - [After solving on your own, see solution here](./Solutions/8_4_Solution3.html)


## Technology
The videos below were seen in 8.3 on correlation. When we calculated the correlation coefficient $$r$$, we also found the coefficient of determination $$r^2$$. The videos are here as a reminder to you.

### TI-83/84
1. Turn on Diagnostics (only needs to be done once)
  - Press **2nd**
  - Press **0** (CATALOG)
  - Scroll down to **DiagnosticOn**
  - Press **ENTER** twice.
2. Press **STAT**, then select **1: Edit**, and enter your $x$-values into **L1** and your $y$-values into **L2**.
3. Press **STAT**, arrow over to **CALC**, and select **4: LinReg(ax+b)**.
4. Set **Xlist** to **L1** and **Ylist** to **L2**, then select **Calculate** and press **ENTER**.
5. Scroll down through the output to find **r²**, listed directly below **r**.

<iframe width="560" height="315" src="https://www.youtube.com/embed/40bG6YErzGA?si=OXEAR5CZAPFfleFU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


### Excel
1. Enter your $x$-values in one column (for example, column A) and your $y$-values in the adjacent column (column B).
2. Click on an empty cell and enter:
   `=RSQ(B1:B10, A1:A10)`
   (Adjust the cell range to match wherever your data is located. Note that `RSQ` wants the $y$-values listed first, then the $x$-values.)
3. This returns the coefficient of determination $r^2$ directly.
4. Alternatively, if you already found $r$ using `CORREL` (see 8.3), you can simply square that result: `=CORREL(A1:A10, B1:B10)^2`
5. You can also see $r^2$ displayed directly on a scatterplot's trendline by checking **Display R-squared value on chart** (see 8.1).


### Desmos
1. Go to [desmos.com/calculator](https://www.desmos.com/calculator).
2. Enter your data into a table, with $x$-values in the first column and $y$-values in the second column (see 8.1 for details).
3. On a new line, run the regression: `y1 ~ a*x1 + b`
4. Click on the small gray box to the left of the regression line to expand the statistics. Desmos displays $r^2$ automatically beneath the regression equation.

This video was shown in 8.1 on the Line of Best Fit. It is good to watch again, but if you are shaky with line of best fit, go ahead and watch it again. You'll see the correlation in the calculation as I mention in the video.

<iframe width="560" height="315" src="https://www.youtube.com/embed/tdikTkheCfs?si=BVpObVSk4ApqxVMw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>