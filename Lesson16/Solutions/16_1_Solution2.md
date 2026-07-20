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
<title>Solution for practice 16.1.2</title>
</head>

## 16.1 Practice Calculating Probabilities - Solution for Practice 2
2. SAT Math scores are approximately normally distributed with $\mu = 520$ and $\sigma = 100$. Find the probability that a randomly selected student scores **more than 650**.

### Solution

This is a "greater than" question, so we find the area to the left, then subtract from 1.

$$z = \frac{650 - 520}{100} = \frac{130}{100} = 1.3$$

$$P(z > 1.3) = 1 - P(z < 1.3) = 1 - 0.9032 = 0.0968$$

The probability that a randomly selected student scores more than 650 is about **0.0968, or 9.68%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson16/16_1_Probabilities.html#practice)
