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
<title>Solution for practice 8.2.3</title>
</head>

## 8.2 Predictions - Solution for Practice 3

3. In 8.1, we found the line of best fit for temperature ($x$, ranging from 60°F to 100°F) and ice cream sales ($y$, in $100s): $y = -8.2 + 0.17x$.
{:start="3"}
  - Predict the ice cream sales on a day when the temperature is 75°F. Is this an interpolation or an extrapolation?
  - Predict the ice cream sales on a day when the temperature is 30°F. Is this an interpolation or an extrapolation? Does the result make sense in context?

### Solution

**Prediction at 75°F**

Substitute $x = 75$ into the line of best fit:

$$y = -8.2 + 0.17(75) = -8.2 + 12.75 = 4.55$$

The predicted ice cream sales are approximately **$455** (4.55 hundred dollars).

Since the original data ranged from 60°F to 100°F, and $x=75$ falls **within** that range, this is an **interpolation**. This prediction is reasonably safe to trust.

**Prediction at 30°F**

Substitute $x = 30$ into the line of best fit:

$$y = -8.2 + 0.17(30) = -8.2 + 5.1 = -3.1$$

The predicted ice cream sales are approximately **-$310** (-3.1 hundred dollars).

Since $x=30$ falls **outside** the original range of 60°F to 100°F, this is an **extrapolation**. And in this case, the result clearly **doesn't make sense**: a shop cannot have negative sales. This is a good example of why extrapolation is risky — the linear pattern observed between 60°F and 100°F doesn't necessarily hold at much colder temperatures, where sales might simply level off near $0 instead of continuing to fall in a straight line. This impossible result is a red flag that the model shouldn't be trusted this far outside the data.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_2_Predictions.html#practice)
