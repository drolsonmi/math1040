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
<title>Solution for practice 13.2.1</title>
</head>

## 13.2 Binomial Probabilities - Solution for Practice 1
1. A fair coin is flipped 6 times. Find the probability of getting exactly 4 heads.

### Solution

Identify the values: $n=6$, $p=0.5$, $q=0.5$, $x=4$.

$$P(4) = \binom{6}{4}(0.5)^4(0.5)^2$$

**Step 1: Find the combination.**

$$\binom{6}{4} = \frac{6!}{4!2!} = 15$$

**Step 2: Find the probability powers.**

$$(0.5)^4 = 0.0625 \qquad (0.5)^2 = 0.25$$

**Step 3: Multiply everything together.**

$$P(4) = 15(0.0625)(0.25) = 0.2344$$

The probability of getting exactly 4 heads in 6 flips is about **23.44%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_2_BinomialProbabilities.html#practice)
