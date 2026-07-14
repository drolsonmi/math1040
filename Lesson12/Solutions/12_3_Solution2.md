<head>
<title>Solution for practice 12.3.2</title>
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

## 12.3 Expected Value - Solution for Practice 2

1. A company surveys 100 customers about their satisfaction with a new product. Assign a numerical value to each category (0 through 4, in order), find the expected value, and interpret what it means.

| Category | Very Unsatisfied | Unsatisfied | Neutral | Satisfied | Very Satisfied |
| --- | --- | --- | --- | --- | --- |
| Count | 5 | 10 | 20 | 40 | 25 |

### Solution

**Step 1: Assign values in order**, since satisfaction is an ordinal variable (there's a clear low-to-high order to the categories).

| Category | Very Unsatisfied | Unsatisfied | Neutral | Satisfied | Very Satisfied |
| --- | --- | --- | --- | --- | --- |
| Value ($x$) | 0 | 1 | 2 | 3 | 4 |

**Step 2: Find the probability of each category** by dividing each count by the total (100 customers).

| Category | Very Unsatisfied | Unsatisfied | Neutral | Satisfied | Very Satisfied |
| --- | --- | --- | --- | --- | --- |
| Probability ($P(x)$) | 5/100 = 0.05 | 10/100 = 0.10 | 20/100 = 0.20 | 40/100 = 0.40 | 25/100 = 0.25 |

**Step 3: Multiply each value by its probability.**

| Category | Very Unsatisfied | Unsatisfied | Neutral | Satisfied | Very Satisfied |
| --- | --- | --- | --- | --- | --- |
| $x \cdot P(x)$ | $0(0.05)=0$ | $1(0.10)=0.10$ | $2(0.20)=0.40$ | $3(0.40)=1.20$ | $4(0.25)=1.00$ |

**Step 4: Add up the results.**

$$E[x] = 0 + 0.10 + 0.40 + 1.20 + 1.00 = 2.70$$

**Interpretation**: The expected value is **2.70**. Since 2 represents "Neutral" and 3 represents "Satisfied," an expected value of 2.70 falls between these two categories, much closer to "Satisfied" than to "Neutral." On average, customers lean toward being satisfied with the product, though not quite at the "Very Satisfied" level.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson12/12_3_ExpectedValue.html#practice)
