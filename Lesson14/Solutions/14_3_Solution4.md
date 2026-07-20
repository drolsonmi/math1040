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
<title>Solution for practice 14.3.4</title>
</head>

## 14.3 Cumulative Binomial Probabilities - Solution for Practice 4
4. A survey shows that 40% of adults in a town support a proposed tax increase. If 15 adults are randomly and independently selected, find the probability that **more than 8** support the increase.

### Solution

Here $n=15$, $p=0.40$, $q=0.60$. "More than 8" is a strict inequality, so it means $P(x\geq 9) = 1-P(x\leq 8)$.

Adding up $P(0)$ through $P(8)$ using the binomial formula (best done with technology to avoid a lengthy hand calculation):

$$P(x\leq 8) \approx 0.9050$$

$$P(x\geq 9) = 1-0.9050 = 0.0950$$

There is about a **9.50%** chance that more than 8 of the 15 adults support the tax increase.

**Check with technology:** On the TI-84, `1 - binomcdf(15, 0.4, 8)` returns approximately 0.0950. ✓

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_3_CumulativeBinomialProbabilities.html#practice)
