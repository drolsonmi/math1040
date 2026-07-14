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
<title>Solution for practice 13.1.3</title>
</head>

## 13.1 Review of "OR" Probabilities - Solution for Practice 3
3. A die is rolled once. Let event $A$ = "rolling an even number" and event $B$ = "rolling a number greater than 4." Are $A$ and $B$ mutually exclusive? Find $P(A \text{ or } B)$.

### Solution

**Step 1: List the outcomes in each event.**

$$A = \{2, 4, 6\} \qquad B = \{5, 6\}$$

**Step 2: Check whether $A$ and $B$ are mutually exclusive.**

The number 6 appears in *both* $A$ and $B$ — it's even, and it's greater than 4. Since $A$ and $B$ share an outcome, they are **not mutually exclusive**. This means we must use the *general* addition rule, not the simplified version.

**Step 3: Find each probability.**

$$P(A) = \frac{3}{6} \qquad P(B) = \frac{2}{6} \qquad P(A \text{ and } B) = \frac{1}{6}$$

($A$ and $B$ overlap only on the outcome $\{6\}$, so $P(A \text{ and } B) = \frac{1}{6}$.)

**Step 4: Apply the general addition rule.**

$$P(A \text{ or } B) = P(A) + P(B) - P(A \text{ and } B)$$

$$P(A \text{ or } B) = \frac{3}{6} + \frac{2}{6} - \frac{1}{6} = \frac{4}{6} = \frac{2}{3} \approx 0.667$$

Notice that if we had mistakenly treated $A$ and $B$ as mutually exclusive and just added $\frac{3}{6}+\frac{2}{6} = \frac{5}{6}$, we would have **double-counted** the outcome 6. This is exactly why it's important to check for mutual exclusivity before choosing which version of the addition rule to use.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_1_ORProbabilities.html#practice)
