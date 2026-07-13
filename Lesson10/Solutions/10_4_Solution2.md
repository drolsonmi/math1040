<head>
<title>Solution for practice 10.4.2</title>
<script>
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']]
  }
};
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## 10.4 AND Probabilities - Solution for Practice 2

1. A bag contains 5 red marbles and 3 blue marbles. Two marbles are drawn **without replacement**. Find $P(\text{first is blue AND second is red})$.

### Solution

**Step 1: Find $P(\text{first blue})$.** The bag starts with 8 marbles total, 3 of which are blue.

$$P(\text{first blue}) = \frac{3}{8}$$

**Step 2: Find $P(\text{second red} \mid \text{first blue})$.** Since the first marble (blue) is not returned to the bag, 7 marbles remain: 5 red and 2 blue.

$$P(\text{second red} \mid \text{first blue}) = \frac{5}{7}$$

**Step 3: Apply the multiplication rule.**

$$P(\text{first blue and second red}) = P(\text{first blue}) \cdot P(\text{second red} \mid \text{first blue}) = \frac{3}{8}\cdot\frac{5}{7} = \frac{15}{56} \approx 0.268$$

The probability that the first marble is blue and the second is red is approximately **0.268, or 26.8%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_4_ANDProbabilities.html#practice)
