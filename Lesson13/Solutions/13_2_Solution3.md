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
<title>Solution for practice 13.2.3</title>
</head>

## 13.2 Binomial Probabilities - Solution for Practice 3
3. A manufacturer knows that 5% of the light bulbs it produces are defective. In a random sample of 12 bulbs, find the probability that exactly 2 are defective.

### Solution

Identify the values: $n=12$, $p=0.05$, $q=0.95$, $x=2$.

$$P(2) = \binom{12}{2}(0.05)^2(0.95)^{10}$$

**Step 1: Find the combination.**

$$\binom{12}{2} = \frac{12!}{2!10!} = 66$$

**Step 2: Find the probability powers.**

$$(0.05)^2 = 0.0025 \qquad (0.95)^{10} \approx 0.59874$$

**Step 3: Multiply everything together.**

$$P(2) = 66(0.0025)(0.59874) \approx 0.0988$$

The probability that exactly 2 of the 12 bulbs are defective is about **9.88%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_2_BinomialProbabilities.html#practice)
