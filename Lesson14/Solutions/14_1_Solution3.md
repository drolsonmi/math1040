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
<title>Solution for practice 14.1.3</title>
</head>

## 14.1 Review of OR Probabilities - Solution for Practice 3
3. A discrete random variable $x$ has the probability distribution below.

| $x$ | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.10 | 0.25 | 0.30 | 0.20 | 0.15 |

Find $P(x=2 \text{ or } x=4)$. Explain why you are able to simply add the two probabilities.

### Solution

A single value of a random variable can't simultaneously equal 2 *and* equal 4 — a random variable only takes on one value at a time. This means the events $x=2$ and $x=4$ are **mutually exclusive**, so we can use the simplified addition rule (no overlap to subtract).

$$P(x=2 \text{ or } x=4) = P(2) + P(4) = 0.25 + 0.20 = 0.45$$

There is a **45%** chance that $x$ equals 2 or 4. This is the same idea we will use throughout the rest of this lesson: since the values of a discrete random variable are always mutually exclusive of one another, finding the probability of "this value or that value" is always as simple as adding the individual probabilities.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson14/14_1_ORProbabilities.html#practice)
