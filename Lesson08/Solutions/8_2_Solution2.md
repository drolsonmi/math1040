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
<title>Solution for practice 8.2.2</title>
</head>

## 8.2 Predictions - Solution for Practice 2

2. In 8.1, we found the line of best fit for a car's age ($x$, ranging from 1 to 5 years) and its resale value ($y$, in $1000s): $y = 22.3 - 2.5x$. Use this line to predict the resale value of a car that is 8 years old. Is this an interpolation or an extrapolation? Explain why we should be cautious about trusting this prediction.
{:start="2"}

### Solution

Substitute $x = 8$ into the line of best fit:

$$y = 22.3 - 2.5(8) = 22.3 - 20 = 2.3$$

The predicted resale value is approximately **$2,300**.

**Interpolation or extrapolation?** The original data only covered cars from 1 to 5 years old. Since $x=8$ falls **outside** that range, this is an **extrapolation**.

**Why be cautious?** Extrapolation assumes that the same linear trend continues beyond where we actually have data, but that assumption often breaks down in the real world. In this case, cars typically don't depreciate in a perfectly straight line forever — the rate of depreciation usually slows down as a car gets older, and the value tends to level off near some minimum resale or scrap value rather than continuing to fall at a constant $2,500/year. If we extrapolated even further (say, to $x=12$), the line would predict a resale value of $22.3 - 2.5(12) = -7.7$, or **-$7,700**, which is impossible — a clear sign that the linear model shouldn't be trusted this far outside the original data.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_2_Predictions.html#practice)
