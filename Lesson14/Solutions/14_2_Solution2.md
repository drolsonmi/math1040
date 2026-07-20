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
<title>Solution for practice 14.2.2</title>
</head>

## 14.2 Cumulative Probabilities - Solution for Practice 2

| $x$ | 0 | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.05 | 0.15 | 0.30 | 0.25 | 0.15 | 0.10 |

2. Find the probability that **more than 3** tickets come in during a given hour.

### Solution

"More than 3" means $x > 3$, which is a *strict* inequality, so $x=3$ is **not** included. We add the probabilities for $x=4$ and $x=5$.

$$P(x>3) = P(4)+P(5) = 0.15+0.10 = 0.25$$

There is a **25%** chance that more than 3 tickets come in during a given hour.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_2_CumulativeProbabilities.html#practice)
