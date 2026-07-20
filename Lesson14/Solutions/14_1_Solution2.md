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
<title>Solution for practice 14.1.2</title>
</head>

## 14.1 Review of OR Probabilities - Solution for Practice 2
2. A standard deck of 52 cards is shuffled, and one card is drawn. Find the probability that the card is a Heart **or** a Face card (Jack, Queen, or King).

### Solution

A card can be both a Heart and a Face card at the same time (for example, the Jack of Hearts), so these events are **not mutually exclusive**. We need the general addition rule.

$$P(\text{Heart}) = \frac{13}{52}, \qquad P(\text{Face card}) = \frac{12}{52}, \qquad P(\text{Heart and Face card}) = \frac{3}{52}$$

The last probability comes from the fact that there are exactly 3 face cards that are also hearts: the Jack, Queen, and King of Hearts.

$$P(\text{Heart or Face card}) = \frac{13}{52}+\frac{12}{52}-\frac{3}{52} = \frac{22}{52} = \frac{11}{26} \approx 0.4231$$

There is about a **42.31%** chance of drawing a Heart or a Face card.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_1_ORProbabilities.html#practice)
