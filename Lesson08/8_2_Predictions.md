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

# Lesson 8.2 Linear Regression Predictions
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 8.2.4 Interpreting regression line parameter estimates (pages 352-353)
* 8.2.5 Extrapolation is treacherous (pages 353-354)

## Lesson
There are two ways to use a line of best fit to make predictions
* __Interpolations__ use x-values within the range of your data (somewhere between your data's minimum and maximum)
* __Extrapolations__ use x-values outside the range of your data (somewhere beyond your data's minimum or your data's maximum)

Extra care needs to be taken with extrapolation. Extrapolation assumes that the linear relationship continues beyond your dataset. However, this often isn't the case. So, just be careful whenever you are dealing with extrapolation.

<iframe width="560" height="315" src="https://www.youtube.com/embed/DjDWqFX5vTc?si=J_PNjdQ2WAk0_BFH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. In 8.1, we found the line of best fit for the number of practice sets completed ($x$, ranging from 1 to 5) and a student's quiz score ($y$): $y = 2.3 + 0.9x$. Use this line to predict the quiz score for a student who completes 3.5 practice sets. Is this an interpolation or an extrapolation? Explain.
  - [After solving on your own, see solution here](./Solutions/8_2_Solution1.html)
2. In 8.1, we found the line of best fit for a car's age ($x$, ranging from 1 to 5 years) and its resale value ($y$, in $1000s): $y = 22.3 - 2.5x$. Use this line to predict the resale value of a car that is 8 years old. Is this an interpolation or an extrapolation? Explain why we should be cautious about trusting this prediction.
  - [After solving on your own, see solution here](./Solutions/8_2_Solution2.html)
3. In 8.1, we found the line of best fit for temperature ($x$, ranging from 60°F to 100°F) and ice cream sales ($y$, in $100s): $y = -8.2 + 0.17x$.
  - Predict the ice cream sales on a day when the temperature is 75°F. Is this an interpolation or an extrapolation?
  - Predict the ice cream sales on a day when the temperature is 30°F. Is this an interpolation or an extrapolation? Does the result make sense in context?
  - [After solving on your own, see solution here](./Solutions/8_2_Solution3.html)


## Technology

### TI-83/84

### Excel

### Desmos
