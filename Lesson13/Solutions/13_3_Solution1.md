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
<title>Solution for practice 13.3.1</title>
</head>

## 13.3 Binomial Probability Distribution - Solution for Practice 1
1. A basketball player makes 70% of her free throws. She attempts 5 free throws. Build the full binomial probability distribution table for $X$ = the number of free throws made (list $P(x)$ for $x=0,1,2,3,4,5$), and confirm that the probabilities add up to 1.

### Solution

Here, $n=5$ and $p=0.7$ (so $1-p = 0.3$). We apply the binomial probability formula for every value of $x$ from 0 to 5:

$$P(X=x) = \binom{5}{x}(0.7)^x(0.3)^{5-x}$$

| $x$ | Calculation | $P(x)$ |
| --- | --- | --- |
| 0 | $\binom{5}{0}(0.7)^0(0.3)^5$ | 0.00243 |
| 1 | $\binom{5}{1}(0.7)^1(0.3)^4$ | 0.02835 |
| 2 | $\binom{5}{2}(0.7)^2(0.3)^3$ | 0.13230 |
| 3 | $\binom{5}{3}(0.7)^3(0.3)^2$ | 0.30870 |
| 4 | $\binom{5}{4}(0.7)^4(0.3)^1$ | 0.36015 |
| 5 | $\binom{5}{5}(0.7)^5(0.3)^0$ | 0.16807 |

**Check that the probabilities add up to 1:**

$$0.00243+0.02835+0.13230+0.30870+0.36015+0.16807 = 1.00000$$

The probabilities sum to exactly 1, confirming this is a valid probability distribution. Notice the distribution is skewed toward the higher values of $x$ (4 and 5 made free throws are the most likely outcomes), which makes sense since $p=0.7$ is well above 0.5 — she's more likely to make a free throw than miss it.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_3_BinomialDistribution.html#practice)
