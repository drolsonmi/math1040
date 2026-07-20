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
<title>Solution for practice 13.3.1</title>
</head>

## 13.3 Binomial Distributions - Solution for Practice 1
1. A fair coin is flipped 3 times. Build the complete binomial probability distribution for $x$ = number of heads, and verify that the probabilities sum to 1.

### Solution

Here $n=3$, $p=0.5$, $q=0.5$, and $x$ can be $0,1,2,3$.

$$P(0) = \binom{3}{0}(0.5)^0(0.5)^3 = 1(1)(0.125) = 0.125$$
$$P(1) = \binom{3}{1}(0.5)^1(0.5)^2 = 3(0.5)(0.25) = 0.375$$
$$P(2) = \binom{3}{2}(0.5)^2(0.5)^1 = 3(0.25)(0.5) = 0.375$$
$$P(3) = \binom{3}{3}(0.5)^3(0.5)^0 = 1(0.125)(1) = 0.125$$

| $x$ | 0 | 1 | 2 | 3 |
| --- | --- | --- | --- | --- |
| $P(x)$ | 0.125 | 0.375 | 0.375 | 0.125 |

**Check:** $0.125 + 0.375 + 0.375 + 0.125 = 1.000\checkmark$

The probabilities sum to 1, confirming this is a valid probability distribution.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_3_BinomialDistribution.html#practice)
