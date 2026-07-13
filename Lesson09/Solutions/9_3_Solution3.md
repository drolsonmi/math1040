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
</head>

## 9.3 Complements - Solution for Practice 3

1. A fair six-sided die is rolled once. Let $A$ be the event "rolling less than 3." Find $P(A)$ and $P(A')$, and describe what outcomes make up the complement.

### Solution

**Step 1: Identify event $A$.**

"Rolling less than 3" includes the outcomes 1 and 2:

$$A = \{1, 2\}$$

$$P(A) = \frac{2}{6} = \frac{1}{3} \approx 0.333$$

**Step 2: Find the complement, $A'$.**

The complement of $A$ is every outcome in the sample space that is **not** in $A$ — in other words, "rolling 3 or more":

$$A' = \{3, 4, 5, 6\}$$

**Step 3: Find $P(A')$ using the complement rule.**

$$P(A') = 1 - P(A) = 1 - \frac{1}{3} = \frac{2}{3} \approx 0.667 = 66.7\%$$

**Summary**: $P(A) = \frac{1}{3} \approx 33.3\%$, and $P(A') = \frac{2}{3} \approx 66.7\%$. The complement $A'$ consists of the outcomes $\{3, 4, 5, 6\}$ — every roll that is 3 or higher. As expected, $P(A) + P(A') = \frac{1}{3} + \frac{2}{3} = 1$.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson09/9_3_Complements.html#practice)
