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

# Lesson 8.1 Line of Best Fit
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 8.1.1 Beginning with Straight Lines (pages 340-342)
* 8.1.2 Fitting a line by eye (pages 342)
* 8.1.3 Residuals (pages 342-346)
* 8.2.1 An objective measure for finding the best line (pages 348-349)
* 8.2.2 Conditions for the least squares line (pages 349-350)

## Lesson
Lessons 6 and 7 looked at an analysis of a single quantitative variable. This lesson explores the relationship between two quantitative variables.

We learned [how to create a scatterplot](../Lesson04/4_4_Scatterplots.md) in Lesson 4. Sometimes the scatterplot indicates that relationship between two variables follows a linear pattern. We can draw a line through the middle of the data. This is called a __Line of Best Fit__.

Any line follows the format *y = mx + b* with the slope *m* attached to the variable *x* and the y-intercept  *b* added to that. We will follow the same pattern, but slightly rename the formula.

$$y = a + bx\tag{Line of Best Fit}$$

The trick is finding *a* and *b*. These will be found using a calculator, like a TI-84 or Desmos.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ORm2OOH7l10?si=kVvXtooxM96cEuBO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. A tutor records the number of practice problem sets a student completes and the student's score (out of 10) on the following quiz:
    | Practice Sets Completed ($x$) | 1 | 2 | 3 | 4 | 5 |
    | --- | --- | --- | --- | --- | --- |
    | Quiz Score ($y$) | 3 | 5 | 4 | 6 | 7 |
 
    Find the equation of the line of best fit, $y = a+bx$.
    - [After solving on your own, see solution here](./Solutions/8_1_Solution1.html)

2. A used car dealer records the age of 5 cars (in years) and their resale value (in $1000s):
    | Age of Car ($x$) | 1 | 2 | 3 | 4 | 5 |
    | --- | --- | --- | --- | --- | --- |
    | Resale Value ($y$) | 20 | 17 | 15 | 12 | 10 |
 
    Find the equation of the line of best fit, $y = a+bx$.
    - [After solving on your own, see solution here](./Solutions/8_1_Solution2.html)

3. A researcher records the outdoor temperature (in °F) and a shop's ice cream sales (in $100s) on 5 different days:
    | Temperature ($x$) | 60 | 70 | 80 | 90 | 100 |
    | --- | --- | --- | --- | --- | --- |
    | Ice Cream Sales ($y$) | 2 | 4 | 5 | 7 | 9 |
 
    Find the equation of the line of best fit, $y=a+bx$, and interpret the slope in the context of the problem. Does the y-intercept have a meaningful real-world interpretation here? Explain.
    - [After solving on your own, see solution here](./Solutions/8_1_Solution3.html)


## Technology

### TI-83/84
1. Press **STAT**, then select **1: Edit** to open the list editor.
2. Enter your $x$-values into **L1** and your corresponding $y$-values into **L2** (clear each list first if it already has data, by highlighting the list name and pressing **CLEAR**, then **ENTER**).
3. Press **STAT**, arrow over to **CALC**, and select **4: LinReg(ax+b)**.
4. Set **Xlist** to **L1** and **Ylist** to **L2**, then select **Calculate** and press **ENTER**.
5. The output gives you $a$ (the y-intercept) and $b$ (the slope) directly, so you can write the equation $y = a+bx$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/bj4_aFLUo6M?si=10as9AF0QphbGNeM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


### Excel
1. Enter your $x$-values in one column (for example, column A) and your $y$-values in the adjacent column (column B).
2. To find the slope and y-intercept directly, click on two empty cells and enter:
  - **Slope**: `=SLOPE(B1:B10, A1:A10)`
  - **Intercept**: `=INTERCEPT(B1:B10, A1:A10)`
  (Adjust the cell ranges to match wherever your data is located, with the $y$-values listed first in each formula.)
3. Alternatively, you can see the line of best fit drawn directly on a scatterplot:
  - Select your data and insert a scatterplot chart (**Insert → Chart → Scatter**).
  - Right-click on any data point on the chart and choose **Add Trendline**.
  - In the Trendline options, choose **Linear**, then check the boxes for **Display Equation on chart** and **Display R-squared value on chart**.


### Desmos 
1. Go to [desmos.com/calculator](https://www.desmos.com/calculator).
2. Click on an empty expression line and create a table by typing data directly, or by clicking the **+** button and selecting **table**.
3. Enter your $x$-values in the first column and your $y$-values in the second column.
4. On a new line, type the regression command: `y1 ~ a*x1 + b`
5. Desmos will automatically calculate the values of $a$ and $b$ that best fit your data, and will plot the resulting line on the graph along with your data points.

<iframe width="560" height="315" src="https://www.youtube.com/embed/tdikTkheCfs?si=BVpObVSk4ApqxVMw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>