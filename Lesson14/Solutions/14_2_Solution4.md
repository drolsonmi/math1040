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
<title>Solution for practice 14.2.4</title>
</head>

## 14.2 Cumulative Probabilities - Solution for Practice 4

| $x$ | 0 | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.05 | 0.15 | 0.30 | 0.25 | 0.15 | 0.10 |

4. Find the probability that **at least 1** ticket comes in during a given hour, using the Complement Shortcut.

### Solution

"At least 1" is the complement of "fewer than 1," which is just $x=0$.

$$P(x\geq 1) = 1-P(x\leq 0) = 1-P(0) = 1-0.05 = 0.95$$

There is a **95%** chance that at least 1 ticket comes in during a given hour. Notice how much faster this was than adding up $P(1)+P(2)+P(3)+P(4)+P(5)$ directly — this is exactly why the Complement Shortcut is so useful for "at least" questions.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_2_CumulativeProbabilities.html#practice)
