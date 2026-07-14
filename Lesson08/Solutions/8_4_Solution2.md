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
<title>Solution for practice 8.4.2</title>
</head>

## 8.4 The Coefficient of Determination - Solution for Practice 2

2. In 8.3, we found that the correlation coefficient for the car age vs. resale value data was $r \approx -0.998$. Find the coefficient of determination, $r^2$, and interpret it in the context of this problem.
{:start="2"}

### Solution

$$r^2 = (-0.998)^2 \approx 0.996$$

**Interpretation**: About **99.6%** of the variation in resale value can be explained by the linear relationship with the car's age. This is an extremely high value, meaning the line of best fit is an excellent fit for this data — a car's age almost entirely determines its resale value in this dataset, leaving very little (about 0.4%) of the variation explained by anything else.

Notice that even though the correlation itself was **negative** ($r \approx -0.998$), the coefficient of determination is still **positive**, since squaring a negative number removes the sign. This is a good reminder that $r^2$ only tells us *how much* variation is explained — it never tells us the *direction* of the relationship. We still need to look at $r$ (or the sign of the slope) for that.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_4_CoeffDetermination.html#practice)
