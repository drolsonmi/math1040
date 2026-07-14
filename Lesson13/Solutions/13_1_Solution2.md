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
<title>Solution for practice 13.1.2</title>
</head>

## 13.1 Review of "OR" Probabilities - Solution for Practice 2
2. A jar of marbles contains only red, blue, and green marbles. The probability of drawing a red marble is 0.3, and the probability of drawing a blue marble is 0.45. What is the probability of drawing a red or a blue marble? What is the probability of drawing a green marble?

### Solution

**Part 1: Red or blue**

A single marble can't be both red and blue at the same time, so these events are mutually exclusive:

$$P(\text{red or blue}) = P(\text{red}) + P(\text{blue}) = 0.3 + 0.45 = 0.75$$

There is a **75% chance** of drawing a red or blue marble.

**Part 2: Green**

Since the jar contains *only* red, blue, and green marbles, the probabilities of all three colors must add up to 1 (this is the same idea we used when building probability distributions in lesson 12 — all the probabilities in a distribution add up to 1):

$$P(\text{red}) + P(\text{blue}) + P(\text{green}) = 1$$

$$0.3 + 0.45 + P(\text{green}) = 1$$

$$P(\text{green}) = 1 - 0.75 = 0.25$$

There is a **25% chance** of drawing a green marble.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_1_ORProbabilities.html#practice)
