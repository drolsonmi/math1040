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
<title>Solution for practice 16.1.3</title>
</head>

## 16.1 Practice Calculating Probabilities - Solution for Practice 3
3. Phone battery life is approximately normally distributed with $\mu = 11$ hours and $\sigma = 1.2$ hours. Find the probability that a randomly selected phone's battery lasts **between 9 and 12 hours**.

### Solution

This is a "between" question, so we find both z-scores and subtract the smaller area from the larger one.

$$z_a = \frac{9 - 11}{1.2} = \frac{-2}{1.2} \approx -1.67 \qquad z_b = \frac{12 - 11}{1.2} = \frac{1}{1.2} \approx 0.83$$

$$P(z < 0.83) = 0.7967 \qquad P(z < -1.67) = 0.0475$$

$$P(-1.67 < z < 0.83) = 0.7967 - 0.0475 = 0.7492$$

The probability that a randomly selected phone's battery lasts between 9 and 12 hours is about **0.7492, or 74.92%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson16/16_1_Probabilities.html#practice)
