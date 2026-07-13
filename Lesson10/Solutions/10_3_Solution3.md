<head>
<title>Solution for practice 10.3.3</title>
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

## 10.3 Conditional Probabilities - Solution for Practice 3

1. A single card is drawn from a standard 52-card deck. There are 12 face cards (Jacks, Queens, and Kings) in the deck. Find $P(\text{King} \mid \text{face card})$.

### Solution

Since we're told the card is a face card, we restrict our attention to just the 12 face cards, and ask how many of those 12 are Kings (4):

$$P(\text{King} \mid \text{face card}) = \frac{4}{12} = \frac{1}{3} \approx 0.333$$

We get the same result using the formula directly. Every King is automatically also a face card, so $P(\text{King and face card}) = P(\text{King}) = \frac{4}{52}$:

$$P(\text{King} \mid \text{face card}) = \frac{P(\text{King and face card})}{P(\text{face card})} = \frac{4/52}{12/52} = \frac{4}{12} = \frac{1}{3}$$

The probability of drawing a King, given that the card is a face card, is approximately **0.333, or 33.3%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_3_ConditionalProbabilities.html#practice)
