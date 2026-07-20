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
<title>Solution for practice 14.2.1</title>
</head>

## 14.2 Cumulative Probabilities - Solution for Practice 1

| $x$ | 0 | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.05 | 0.15 | 0.30 | 0.25 | 0.15 | 0.10 |

1. Find the probability that **at most 2** tickets come in during a given hour.

### Solution

"At most 2" means $x \leq 2$, so we add the probabilities for $x=0, 1,$ and $2$.

$$P(x\leq 2) = P(0)+P(1)+P(2) = 0.05+0.15+0.30 = 0.50$$

There is a **50%** chance that at most 2 tickets come in during a given hour.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_2_CumulativeProbabilities.html#practice)
