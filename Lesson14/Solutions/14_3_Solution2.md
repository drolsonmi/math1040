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
<title>Solution for practice 14.3.2</title>
</head>

## 14.3 Cumulative Binomial Probabilities - Solution for Practice 2
2. Historically, 15% of packages shipped by a company arrive late. For a random sample of 20 independent packages, find the probability that **at least 5** arrive late.

### Solution

Here $n=20$, $p=0.15$, $q=0.85$. "At least 5" is $P(x\geq 5)$, which we'll find using the Complement Shortcut:

$$P(x\geq 5) = 1-P(x\leq 4)$$

Calculate the terms of $P(x\leq 4)$:

$$P(0) = \binom{20}{0}(0.15)^0(0.85)^{20} \approx 0.0388$$
$$P(1) = \binom{20}{1}(0.15)^1(0.85)^{19} \approx 0.1368$$
$$P(2) = \binom{20}{2}(0.15)^2(0.85)^{18} \approx 0.2293$$
$$P(3) = \binom{20}{3}(0.15)^3(0.85)^{17} \approx 0.2428$$
$$P(4) = \binom{20}{4}(0.15)^4(0.85)^{16} \approx 0.1821$$

$$P(x\leq 4) \approx 0.0388+0.1368+0.2293+0.2428+0.1821 = 0.8298$$

$$P(x\geq 5) = 1-0.8298 = 0.1702$$

There is about a **17.02%** chance that at least 5 of the 20 packages arrive late.

**Check with technology:** On the TI-84, `1 - binomcdf(20, 0.15, 4)` returns approximately 0.1702. ✓

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_3_CumulativeBinomialProbabilities.html#practice)
