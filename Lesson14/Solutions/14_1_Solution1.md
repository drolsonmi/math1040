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
<title>Solution for practice 14.1.1</title>
</head>

## 14.1 Review of OR Probabilities - Solution for Practice 1
1. A standard deck of 52 cards is shuffled, and one card is drawn. Find the probability that the card is a King **or** a Queen.

### Solution

A card cannot be both a King and a Queen at the same time, so these events are **mutually exclusive**. We can simply add the probabilities.

$$P(\text{King}) = \frac{4}{52}, \qquad P(\text{Queen}) = \frac{4}{52}$$

$$P(\text{King or Queen}) = \frac{4}{52}+\frac{4}{52} = \frac{8}{52} = \frac{2}{13} \approx 0.1538$$

There is about a **15.38%** chance of drawing a King or a Queen.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_1_ORProbabilities.html#practice)
