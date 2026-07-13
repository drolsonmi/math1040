<head>
<title>Solution for practice 10.1.4</title>
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

## 10.1 OR Probabilities - Solution for Practice 4

1. A factory inspects 300 items for two types of defects. 40 items have Defect A, 50 items have Defect B, and 15 items have both defects. Find the probability that a randomly selected item has **Defect A OR Defect B**.

### Solution

**Step 1: Find each individual probability.**

$$P(A) = \frac{40}{300}, \qquad P(B) = \frac{50}{300}$$

**Step 2: Identify the overlap** — items with both defects.

$$P(A \text{ and } B) = \frac{15}{300}$$

**Step 3: Apply the general addition rule.**

$$P(A \text{ or } B) = P(A) + P(B) - P(A \text{ and } B) = \frac{40}{300} + \frac{50}{300} - \frac{15}{300} = \frac{75}{300} = 0.25$$

The probability that a randomly selected item has Defect A or Defect B is **0.25, or 25%**.

**Note**: Without subtracting the overlap, we would have gotten $\frac{90}{300} = 0.30$, which double-counts the 15 items that have *both* defects. Subtracting the overlap corrects for this.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_1_ORProbabilities.html#practice)
