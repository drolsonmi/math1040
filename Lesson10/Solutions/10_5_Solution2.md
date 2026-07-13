<head>
<title>Solution for practice 10.5.2</title>
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

## 10.5 Independent Events - Solution for Practice 2

1. A fair coin is flipped, and a fair six-sided die is rolled. Show that these two events are independent by comparing $P(\text{6})$ to $P(\text{6} \mid \text{heads})$, then use the simplified multiplication rule to find $P(\text{tails AND rolling a 3})$.

### Solution

**Step 1: Show independence.** The coin and the die don't interact with each other in any way, so knowing the coin landed heads gives us no new information about the die:

$$P(6) = \frac{1}{6}, \qquad P(6 \mid \text{heads}) = \frac{1}{6}$$

Since $P(6) = P(6 \mid \text{heads})$, the two events are **independent**.

**Step 2: Use the simplified multiplication rule.** Because the events are independent, we can multiply the plain probabilities directly, without needing a conditional probability:

$$P(\text{tails and 3}) = P(\text{tails}) \cdot P(3) = \frac{1}{2}\cdot\frac{1}{6} = \frac{1}{12} \approx 0.0833$$

The probability of flipping tails and rolling a 3 is approximately **0.083, or 8.3%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_5_IndependentEvents.html#practice)
