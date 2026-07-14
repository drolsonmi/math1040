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

## 13.3 Binomial Probability Distribution - Solution for Practice 3
3. A call center finds that 25% of incoming calls result in a sale. Out of 15 randomly selected calls, what is the probability that **6, 7, or 8** of them result in a sale?

### Solution

**Step 1: Identify $n$ and $p$.**

- $n = 15$
- $p = 0.25$ (probability a call results in a sale)

We need $P(X=6)+P(X=7)+P(X=8)$, since these three outcomes are mutually exclusive.

**Step 2: Calculate each individual probability.**

$$P(X=6) = \binom{15}{6}(0.25)^6(0.75)^9 = 5005 \times 0.000244140625 \times 0.075084686\ldots \approx 0.09175$$

$$P(X=7) = \binom{15}{7}(0.25)^7(0.75)^8 = 6435 \times 0.00006103515625 \times 0.100112915\ldots \approx 0.03932$$

$$P(X=8) = \binom{15}{8}(0.25)^8(0.75)^7 = 6435 \times 0.0000152587890625 \times 0.133483887\ldots \approx 0.01311$$

**Step 3: Add the probabilities together.**

$$P(6 \le X \le 8) = 0.09175+0.03932+0.01311 \approx 0.1442$$

There is about a **14.4% chance** that 6, 7, or 8 out of the 15 calls result in a sale.

Note that the average (expected) number of sales here is $n\cdot p = 15 \times 0.25 = 3.75$, so 6, 7, and 8 are all noticeably above average — which is why this combined probability is relatively small. If you'd like to check this answer quickly, try it with your calculator's cumulative binomial function (`binomcdf(15, 0.25, 8) - binomcdf(15, 0.25, 5)`), covered in the Technology section of the lesson.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_3_BinomialDistribution.html#practice)
