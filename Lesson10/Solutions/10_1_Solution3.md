<head>
<title>Solution for practice 10.1.3</title>
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

## 10.1 OR Probabilities - Solution for Practice 3

1. A fair six-sided die is rolled once. Find $P(\text{rolling an even number OR rolling a number greater than 4})$.

### Solution

**Step 1: Identify each event.**

$$\text{Even} = \{2, 4, 6\}, \qquad \text{Greater than 4} = \{5, 6\}$$

$$P(\text{even}) = \frac{3}{6}, \qquad P(\text{greater than 4}) = \frac{2}{6}$$

**Step 2: Find the overlap.** The number 6 appears in both events (it's even, and it's greater than 4).

$$P(\text{even and greater than 4}) = \frac{1}{6}$$

**Step 3: Apply the general addition rule.**

$$P(\text{even or greater than 4}) = \frac{3}{6} + \frac{2}{6} - \frac{1}{6} = \frac{4}{6} = \frac{2}{3} \approx 0.667$$

The probability is approximately **0.667, or 66.7%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_1_ORProbabilities.html#practice)
