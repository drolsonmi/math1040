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
<title>Solution for practice 13.1.2</title>
</head>

## 13.1 What is a Binomial Distribution? - Solution for Practice 2
2. A bag contains 4 red marbles and 2 blue marbles. Three marbles are drawn **without replacement**, and we count the number of red marbles drawn.

### Solution

Check the four requirements:
- Fixed number of trials: yes, $n=3$ draws.
- Two outcomes: yes, each draw is red (success) or blue (failure).
- Constant probability: **no**. On the first draw, $P(\text{red}) = \frac{4}{6}$. If a red marble is drawn first, the probability of red on the second draw drops to $\frac{3}{5}$. Since marbles are not replaced, the probability of success changes from draw to draw.
- Independent trials: **no**, for the same reason — what happens on one draw changes what is left in the bag for the next draw.

Because the probability of success is not constant and the draws are not independent, this **is not a binomial experiment**. (With a bag this small, removing even one marble noticeably changes the probabilities, so we cannot use the "large population" approximation either.)

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_1_WhatIsBinomial.html#practice)
