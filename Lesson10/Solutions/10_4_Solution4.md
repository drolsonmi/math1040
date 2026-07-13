<head>
<title>Solution for practice 10.4.4</title>
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

## 10.4 AND Probabilities - Solution for Practice 4

1. A fair coin is flipped, and a fair six-sided die is rolled. These two events don't affect each other at all. Find $P(\text{coin shows heads AND die shows a 6})$.

### Solution

Since the coin flip and the die roll don't affect each other, knowing the result of the coin flip tells us nothing new about the die. This means:

$$P(\text{6} \mid \text{heads}) = P(\text{6}) = \frac{1}{6}$$

Applying the multiplication rule:

$$P(\text{heads and 6}) = P(\text{heads}) \cdot P(\text{6} \mid \text{heads}) = \frac{1}{2}\cdot\frac{1}{6} = \frac{1}{12} \approx 0.0833$$

The probability of flipping heads and rolling a 6 is approximately **0.083, or 8.3%**.

**Note**: Because the conditional probability $P(6 \mid \text{heads})$ turned out to be exactly the same as the plain probability $P(6)$, we could have just multiplied $P(\text{heads}) \cdot P(6)$ directly, without worrying about the "given that" part at all. Events that behave this way are called **independent events** — the focus of 10.5.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_4_ANDProbabilities.html#practice)
