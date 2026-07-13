<head>
<title>Solution for practice 10.4.3</title>
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

## 10.4 AND Probabilities - Solution for Practice 3

1. Two cards are drawn **without replacement** from a standard 52-card deck. Find $P(\text{both cards are Kings})$.

### Solution

**Step 1: Find $P(\text{first is a King})$.** There are 4 Kings in a 52-card deck.

$$P(\text{first King}) = \frac{4}{52}$$

**Step 2: Find $P(\text{second is a King} \mid \text{first is a King})$.** Since the first King is not returned to the deck, 51 cards remain, only 3 of which are Kings.

$$P(\text{second King} \mid \text{first King}) = \frac{3}{51}$$

**Step 3: Apply the multiplication rule.**

$$P(\text{both Kings}) = \frac{4}{52}\cdot\frac{3}{51} = \frac{12}{2652} = \frac{1}{221} \approx 0.00452$$

The probability of drawing two Kings in a row (without replacement) is approximately **0.0045, or 0.45%** — quite rare, which makes sense since there are only 4 Kings in the whole deck.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_4_ANDProbabilities.html#practice)
