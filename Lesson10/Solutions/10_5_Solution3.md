<head>
<title>Solution for practice 10.5.3</title>
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

## 10.5 Independent Events - Solution for Practice 3

1. Compare drawing two cards **with replacement** vs. **without replacement**, and explain why one produces independent events while the other does not.

### Solution

**Scenario A: With replacement.** The first card is drawn, then put back into the deck before the second draw. This means the deck is back to its full 52 cards (including all 4 Kings) for the second draw, regardless of what the first card was:

$$P(\text{second King} \mid \text{first King}) = \frac{4}{52} = \frac{1}{13}$$

This is exactly the same as the unconditional probability, $P(\text{King}) = \frac{4}{52} = \frac{1}{13}$. Since $P(\text{second King} \mid \text{first King}) = P(\text{second King})$, **the two draws are independent** when we sample with replacement.

**Scenario B: Without replacement.** The first card is drawn and **not** returned to the deck. If the first card was a King, only 51 cards remain, with only 3 Kings left:

$$P(\text{second King} \mid \text{first King}) = \frac{3}{51} \approx 0.0588$$

This is different from $P(\text{King}) = \frac{4}{52} \approx 0.0769$. Since these values are **not equal**, **the two draws are dependent** when we sample without replacement.

**Why the difference?** Sampling **with replacement** resets the sample space after every draw, so nothing about earlier draws affects later ones — this is what makes the draws independent. Sampling **without replacement** permanently removes an item from the sample space, so every draw changes what's available for the next one — this dependency is exactly why we needed the general (not simplified) multiplication rule back in 10.4.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_5_IndependentEvents.html#practice)
