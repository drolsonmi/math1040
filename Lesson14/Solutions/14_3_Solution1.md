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
<title>Solution for practice 14.3.1</title>
</head>

## 14.3 Cumulative Binomial Probabilities - Solution for Practice 1
1. A fair coin is flipped 10 times. Find the probability of getting **at most 4** heads.

### Solution

Here $n=10$, $p=0.5$, $q=0.5$, and we need $P(x\leq 4) = P(0)+P(1)+P(2)+P(3)+P(4)$.

$$P(0) = \binom{10}{0}(0.5)^0(0.5)^{10} \approx 0.0010$$
$$P(1) = \binom{10}{1}(0.5)^1(0.5)^{9} \approx 0.0098$$
$$P(2) = \binom{10}{2}(0.5)^2(0.5)^{8} \approx 0.0439$$
$$P(3) = \binom{10}{3}(0.5)^3(0.5)^{7} \approx 0.1172$$
$$P(4) = \binom{10}{4}(0.5)^4(0.5)^{6} \approx 0.2051$$

$$P(x\leq 4) \approx 0.0010+0.0098+0.0439+0.1172+0.2051 = 0.3770$$

There is about a **37.70%** chance of getting at most 4 heads in 10 flips.

**Check with technology:** On the TI-84, `binomcdf(10, 0.5, 4)` returns approximately 0.3770. ✓

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_3_CumulativeBinomialProbabilities.html#practice)
