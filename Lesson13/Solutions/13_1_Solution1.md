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
<title>Solution for practice 13.1.1</title>
</head>

## 13.1 What is a Binomial Distribution? - Solution for Practice 1
1. A fair coin is flipped 10 times, and we count the number of heads.

### Solution

Check the four requirements:
- Fixed number of trials: yes, $n=10$ flips are set in advance.
- Two outcomes: yes, each flip is heads (success) or tails (failure).
- Constant probability: yes, each flip has the same probability of heads, since the coin doesn't change between flips.
- Independent trials: yes, the outcome of one flip has no effect on any other flip.

All four requirements are met, so this **is a binomial experiment**.

$$n = 10 \qquad p = 0.5 \qquad q = 1-0.5 = 0.5$$

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_1_WhatIsBinomial.html#practice)
