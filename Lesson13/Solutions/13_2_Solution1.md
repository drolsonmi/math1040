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
1. A fair coin is flipped 8 times. What is the probability of getting exactly 5 heads?

### Solution

**Step 1: Identify $n$, $p$, and $k$.**

- $n = 8$ (8 flips)
- $p = 0.5$ (probability of heads on a fair coin)
- $k = 5$ (we want exactly 5 heads)

**Step 2: Set up the binomial probability formula.**

$$P(X=k) = \binom{n}{k}p^k(1-p)^{n-k}$$

$$P(X=5) = \binom{8}{5}(0.5)^5(0.5)^3$$

**Step 3: Calculate the combination.**

$$\binom{8}{5} = \frac{8!}{5!\,3!} = 56$$

**Step 4: Calculate the powers and multiply.**

$$P(X=5) = 56 \times (0.5)^5 \times (0.5)^3 = 56 \times 0.03125 \times 0.125$$

$$P(X=5) = 56 \times 0.00390625 \approx 0.2188$$

There is about a **21.9% chance** of getting exactly 5 heads in 8 flips.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_2_BinomialProbabilities.html#practice)
