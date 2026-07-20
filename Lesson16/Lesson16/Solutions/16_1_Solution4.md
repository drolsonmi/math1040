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
<title>Solution for practice 16.1.4</title>
</head>

## 16.1 Practice Calculating Probabilities - Solution for Practice 4
4. Daily household water usage is approximately normally distributed with $\mu = 300$ gallons and $\sigma = 40$ gallons. Find the probability that a randomly selected household uses **more than 380 gallons** in a day.

### Solution

This is a "greater than" question, so we find the area to the left, then subtract from 1.

$$z = \frac{380 - 300}{40} = \frac{80}{40} = 2.00$$

$$P(z > 2.00) = 1 - P(z < 2.00) = 1 - 0.9772 = 0.0228$$

The probability that a randomly selected household uses more than 380 gallons in a day is about **0.0228, or 2.28%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson16/16_1_Probabilities.html#practice)
