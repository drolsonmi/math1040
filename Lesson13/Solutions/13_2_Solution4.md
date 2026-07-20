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
<title>Solution for practice 13.2.4</title>
</head>

## 13.2 Binomial Probabilities - Solution for Practice 4
4. According to a survey, 65% of adults in a city support a new recycling program. If 9 adults are randomly and independently selected, find the probability that exactly 6 of them support the program.

### Solution

Identify the values: $n=9$, $p=0.65$, $q=0.35$, $x=6$.

$$P(6) = \binom{9}{6}(0.65)^6(0.35)^3$$

**Step 1: Find the combination.**

$$\binom{9}{6} = \frac{9!}{6!3!} = 84$$

**Step 2: Find the probability powers.**

$$(0.65)^6 \approx 0.07542 \qquad (0.35)^3 \approx 0.04288$$

**Step 3: Multiply everything together.**

$$P(6) = 84(0.07542)(0.04288) \approx 0.2717$$

The probability that exactly 6 of the 9 adults support the program is about **27.17%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_2_BinomialProbabilities.html#practice)
