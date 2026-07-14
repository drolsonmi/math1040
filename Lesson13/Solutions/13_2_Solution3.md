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
3. Historically, 85% of flights at a small airport depart on time. If 6 flights are selected at random, what is the probability that exactly 4 of them departed on time?

### Solution

**Step 1: Identify $n$, $p$, and $k$.**

- $n = 6$
- $p = 0.85$ (probability a flight departs on time — this is our "success")
- $k = 4$

**Step 2: Set up the binomial probability formula.**

$$P(X=4) = \binom{6}{4}(0.85)^4(0.15)^2$$

**Step 3: Calculate the combination.**

$$\binom{6}{4} = \frac{6!}{4!\,2!} = 15$$

**Step 4: Calculate the powers and multiply.**

$$(0.85)^4 \approx 0.52200 \qquad (0.15)^2 = 0.0225$$

$$P(X=4) = 15 \times 0.52200 \times 0.0225 \approx 0.1762$$

There is about a **17.6% chance** that exactly 4 of the 6 randomly selected flights departed on time.

Notice that this probability is fairly low even though 85% of flights are on time individually — that's because we're asking for *exactly* 4, not "4 or more." A result of 5 or 6 on-time flights is actually more likely here, since $p=0.85$ is closer to 1, and $n=6$ is small. We'll build the full distribution for a situation like this in the next lesson.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_2_BinomialProbabilities.html#practice)
