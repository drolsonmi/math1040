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
<title>Solution for practice 14.3.3</title>
</head>

## 14.3 Cumulative Binomial Probabilities - Solution for Practice 3
3. A basketball player makes 75% of her free throws. If she shoots 12 free throws, find the probability that she makes **between 8 and 10** (inclusive).

### Solution

Here $n=12$, $p=0.75$, $q=0.25$. "Between 8 and 10, inclusive" means $P(8\leq x\leq 10) = P(8)+P(9)+P(10)$.

$$P(8) = \binom{12}{8}(0.75)^8(0.25)^4 \approx 0.1936$$
$$P(9) = \binom{12}{9}(0.75)^9(0.25)^3 \approx 0.2581$$
$$P(10) = \binom{12}{10}(0.75)^{10}(0.25)^2 \approx 0.2323$$

$$P(8\leq x\leq 10) \approx 0.1936+0.2581+0.2323 = 0.6840$$

There is about a **68.40%** chance that she makes between 8 and 10 of her 12 free throws.

**Check with technology:** On the TI-84, `binomcdf(12, 0.75, 10) - binomcdf(12, 0.75, 7)` returns approximately 0.6840. ✓

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_3_CumulativeBinomialProbabilities.html#practice)
