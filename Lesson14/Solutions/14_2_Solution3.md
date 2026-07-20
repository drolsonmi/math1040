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
<title>Solution for practice 14.2.3</title>
</head>

## 14.2 Cumulative Probabilities - Solution for Practice 3

| $x$ | 0 | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.05 | 0.15 | 0.30 | 0.25 | 0.15 | 0.10 |

3. Find the probability that **between 1 and 3** tickets (inclusive) come in during a given hour.

### Solution

"Between 1 and 3, inclusive" means $1 \leq x \leq 3$, so we add the probabilities for $x=1, 2,$ and $3$.

$$P(1\leq x\leq 3) = P(1)+P(2)+P(3) = 0.15+0.30+0.25 = 0.70$$

There is a **70%** chance that between 1 and 3 tickets (inclusive) come in during a given hour.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_2_CumulativeProbabilities.html#practice)
