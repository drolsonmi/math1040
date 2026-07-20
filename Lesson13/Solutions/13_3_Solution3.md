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
<title>Solution for practice 13.3.3</title>
</head>

## 13.3 Binomial Distributions - Solution for Practice 3
3. A pharmaceutical trial shows that a new medication is effective for 60% of patients. For a group of 4 independent patients, build the complete binomial distribution for $x$ = number for whom the medication is effective. Use the distribution to find $P(x \geq 3)$.

### Solution

Here $n=4$, $p=0.6$, $q=0.4$, and $x$ can be $0,1,2,3,4$.

$$P(0) = \binom{4}{0}(0.6)^0(0.4)^4 = 1(1)(0.0256) = 0.0256$$
$$P(1) = \binom{4}{1}(0.6)^1(0.4)^3 = 4(0.6)(0.064) = 0.1536$$
$$P(2) = \binom{4}{2}(0.6)^2(0.4)^2 = 6(0.36)(0.16) = 0.3456$$
$$P(3) = \binom{4}{3}(0.6)^3(0.4)^1 = 4(0.216)(0.4) = 0.3456$$
$$P(4) = \binom{4}{4}(0.6)^4(0.4)^0 = 1(0.1296)(1) = 0.1296$$

| $x$ | 0 | 1 | 2 | 3 | 4 |
| --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.0256 | 0.1536 | 0.3456 | 0.3456 | 0.1296 |

**Check:** $0.0256+0.1536+0.3456+0.3456+0.1296 = 1.0000\checkmark$

To find $P(x \geq 3)$, we add the probabilities of the outcomes that satisfy $x \geq 3$, namely $x=3$ and $x=4$:

$$P(x\geq 3) = P(3) + P(4) = 0.3456 + 0.1296 = 0.4752$$

There is about a **47.52%** chance that the medication is effective for at least 3 of the 4 patients.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_3_BinomialDistribution.html#practice)
