<head>
<title>Solution for practice 10.1.1</title>
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

## 10.1 OR Probabilities - Solution for Practice 1

1. A single card is drawn from a standard 52-card deck. Find $P(\text{Jack OR Spade})$.

### Solution

**Step 1: Find each individual probability.**

$$P(\text{Jack}) = \frac{4}{52}, \qquad P(\text{Spade}) = \frac{13}{52}$$

**Step 2: Find the overlap.** There is exactly one card that is both a Jack and a Spade — the Jack of Spades.

$$P(\text{Jack and Spade}) = \frac{1}{52}$$

**Step 3: Apply the general addition rule.**

$$P(\text{Jack or Spade}) = P(\text{Jack}) + P(\text{Spade}) - P(\text{Jack and Spade}) = \frac{4}{52} + \frac{13}{52} - \frac{1}{52} = \frac{16}{52} = \frac{4}{13} \approx 0.308$$

The probability of drawing a Jack or a Spade is approximately **0.308, or 30.8%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_1_ORProbabilities.html#practice)
