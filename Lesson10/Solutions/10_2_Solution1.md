<head>
<title>Solution for practice 10.2.1</title>
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

## 10.2 Mutually Exclusive Events - Solution for Practice 1

1. A single card is drawn from a standard 52-card deck. Explain why "drawing a King" and "drawing a Queen" are mutually exclusive, then find $P(\text{King OR Queen})$.

### Solution

**Why mutually exclusive?** A single card can only have one rank. No card in the deck is both a King and a Queen at the same time, so there is no overlap between these two events — they are **mutually exclusive**.

**Finding the probability**: Since $P(\text{King and Queen}) = 0$, the general addition rule simplifies:

$$P(\text{King or Queen}) = P(\text{King}) + P(\text{Queen}) = \frac{4}{52} + \frac{4}{52} = \frac{8}{52} = \frac{2}{13} \approx 0.154$$

The probability of drawing a King or a Queen is approximately **0.154, or 15.4%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_2_MutuallyExclusive.html#practice)
