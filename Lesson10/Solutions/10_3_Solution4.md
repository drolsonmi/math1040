<head>
<title>Solution for practice 10.3.4</title>
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

## 10.3 Conditional Probabilities - Solution for Practice 4

1. A bag contains 5 red marbles and 3 blue marbles. Two marbles are drawn **without replacement**. Find $P(\text{second marble is blue} \mid \text{first marble is red})$.

### Solution

The bag starts with 8 marbles total (5 red, 3 blue). Since we're told the **first** marble drawn was red, and it is **not** put back into the bag, only 7 marbles remain for the second draw: 4 red and 3 blue.

$$P(\text{second blue} \mid \text{first red}) = \frac{3}{7} \approx 0.429$$

The probability that the second marble is blue, given that the first marble drawn was red, is approximately **0.429, or 42.9%**.

**Note**: This is different from the probability of drawing blue on the very first draw, $P(\text{blue}) = \frac{3}{8} = 0.375$. Removing a red marble on the first draw slightly increased the chance of blue on the second draw, since it left proportionally more blue marbles in the bag. This shows how "without replacement" situations naturally create conditional probabilities — we'll use this same setup to calculate an "AND" probability in 10.4.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_3_ConditionalProbabilities.html#practice)
