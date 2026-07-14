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
<title>Solution for practice 13.1.1</title>
</head>

## 13.1 Review of "OR" Probabilities - Solution for Practice 1
1. A survey of registered voters finds that 40% support Proposal A and 25% support Proposal B. No voter supports both proposals (they are mutually exclusive positions). What is the probability that a randomly selected voter supports Proposal A or Proposal B?

### Solution

Since no voter can support both proposals, supporting Proposal A and supporting Proposal B are **mutually exclusive** events. This means we can use the simplified addition rule:

$$P(A \text{ or } B) = P(A) + P(B)$$

We're given:

$$P(A) = 0.40 \qquad P(B) = 0.25$$

$$P(A \text{ or } B) = 0.40 + 0.25 = 0.65$$

There is a **65% chance** that a randomly selected voter supports Proposal A or Proposal B.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_1_ORProbabilities.html#practice)
