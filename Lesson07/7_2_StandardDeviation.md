<head>
<title>Lesson 7.2 Standard Deviation</title>
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

# Lesson 7.2 Standard Deviation
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 2.2.2 Standard deviation as a measure of spread (pages 58-61)

## Lesson
Since we had to square the deviations to find the variance, our result comes out in squared units. To get rid of the squared unit, take the square root. This is the standard deviation.

Variance for a population and a sample

$$\sigma^2 = \frac{\sum(x-\mu)^2}{n} \qquad s^2 = \frac{\sum(x-\bar{x})^2}{n-1}\tag{Variance}$$

Standard Deviation for a population and a sample

$$\sigma = \sqrt{\frac{\sum(x-\mu)^2}{n}} \qquad s = \sqrt{\frac{\sum(x-\bar{x})^2}{n-1}}\tag{Standard Deviation}$$

The standard deviation can be interpreted as a specific distance from the mean that indicates how spread out the data is.

<iframe width="560" height="315" src="https://www.youtube.com/embed/CTPOPyxlqww?si=ofxVUJipldLfpT9B" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. A teacher records the ages of all 5 students in a small tutoring group: $[10, 12, 14, 16, 18]$. Since this is every student in the group, treat this as a **population**. Find the population standard deviation.
  - [After solving on your own, see solution here](./Solutions/7_2_Solution1.html)
2. A researcher records the reaction times (in tenths of a second) of a **sample** of 6 volunteers: $[5, 7, 9, 9, 11, 13]$. Find the sample standard deviation.
  - [After solving on your own, see solution here](./Solutions/7_2_Solution2.html)
3. Two classes take the same 5-question quiz. A sample of scores from each class is recorded:
  - Class A: $[78, 82, 85, 80, 90]$
  - Class B: $[83, 84, 82, 83, 83]$
  - Find the sample standard deviation for each class. Both classes have the same mean — what does the standard deviation tell you about how the two classes differ?
  - [After solving on your own, see solution here](./Solutions/7_2_Solution3.html)

## Technology

### TI-83/84
1. Press **STAT**, then select **1: Edit** to open the list editor.
2. Enter your data values into **L1** (clear the list first if it already has data in it, by highlighting `L1` and pressing **CLEAR**, then **ENTER**).
3. Press **STAT**, arrow over to **CALC**, and select **1: 1-Var Stats**.
4. Make sure the list is set to **L1**, then press **ENTER** (or **Calculate**) to run it.
5. Scroll down through the output:
  - **Sx** is the **sample standard deviation**
  - **σx** is the **population standard deviation**

<iframe width="560" height="315" src="https://www.youtube.com/embed/hq4rMWLt8mo?si=N0u8CgXJj5mlnPLG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Excel
1. Enter your data values into a single column (for example, cells A1 through A10).
2. Click on an empty cell where you want the result to appear.
3. Type one of the following formulas, depending on whether your data is a sample or a population, then press Enter:
  - **Sample standard deviation**: `=STDEV.S(A1:A10)`
  - **Population standard deviation**: `=STDEV.P(A1:A10)`
4. Adjust the cell range (`A1:A10`) to match wherever your data is actually located.