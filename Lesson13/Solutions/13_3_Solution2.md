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
<title>Solution for practice 13.3.2</title>
</head>

## 13.3 Binomial Probability Distribution - Solution for Practice 2
2. A manufacturer finds that 10% of the widgets it produces are defective. In a random sample of 6 widgets, what is the probability that **at most 2** are defective?

### Solution

**Step 1: Identify $n$ and $p$, and translate "at most 2."**

- $n = 6$
- $p = 0.10$ (probability a widget is defective)
- "At most 2" means $X=0$, $X=1$, or $X=2$

Since getting exactly 0, exactly 1, and exactly 2 defective widgets are mutually exclusive outcomes, we can use the addition rule from lesson 13.1:

$$P(X \le 2) = P(X=0)+P(X=1)+P(X=2)$$

**Step 2: Calculate each individual probability.**

$$P(X=0) = \binom{6}{0}(0.1)^0(0.9)^6 = 1 \times 1 \times 0.531441 = 0.531441$$

$$P(X=1) = \binom{6}{1}(0.1)^1(0.9)^5 = 6 \times 0.1 \times 0.59049 = 0.354294$$

$$P(X=2) = \binom{6}{2}(0.1)^2(0.9)^4 = 15 \times 0.01 \times 0.6561 = 0.098415$$

**Step 3: Add the probabilities together.**

$$P(X \le 2) = 0.531441+0.354294+0.098415 = 0.984150$$

There is about a **98.4% chance** that at most 2 of the 6 widgets are defective. This is a high probability, which makes sense since the defect rate is only 10% and we're sampling a small number of widgets — getting 3 or more defective would be unusual.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_3_BinomialDistribution.html#practice)
