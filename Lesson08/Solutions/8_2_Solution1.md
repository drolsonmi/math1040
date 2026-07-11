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
<title>Solution for practice 8.2.1</title>
</head>

## 8.2 Predictions - Solution for Practice 1

1. In 8.1, we found the line of best fit for the number of practice sets completed ($x$, ranging from 1 to 5) and a student's quiz score ($y$): $y = 2.3 + 0.9x$. Use this line to predict the quiz score for a student who completes 3.5 practice sets. Is this an interpolation or an extrapolation? Explain.

### Solution

Substitute $x = 3.5$ into the line of best fit:

$$y = 2.3 + 0.9(3.5) = 2.3 + 3.15 = 5.45$$

The predicted quiz score is approximately **5.45**.

**Interpolation or extrapolation?** The original data ranged from $x=1$ to $x=5$ practice sets. Since $x=3.5$ falls **within** that range, this is an **interpolation**. Interpolations are generally safe to trust, since we're predicting within the range where we actually have data supporting the linear pattern.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_2_Predictions.html#practice)
