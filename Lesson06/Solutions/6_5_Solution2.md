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
<title>Solution for practice 6.5.2</title>
</head>

## 6.5 Boxplots - Solution for Practice 2

1. A dataset has the 5-number summary: Min = 45, Q1 = 52, Median = 60, Q3 = 68, Max = 75.
  - Find the IQR and check for outliers.
  - Based on the box and whisker lengths, describe whether the distribution appears roughly symmetric or skewed.

### Solution

**IQR**: $IQR = Q_3 - Q_1 = 68 - 52 = 16$

**Outlier check**: $1.5 \cdot IQR = 1.5 \cdot 16 = 24$

- Lower fence: $52 - 24 = 28$
- Upper fence: $68 + 24 = 92$

The minimum (45) is above the lower fence (28), and the maximum (75) is below the upper fence (92), so **there are no outliers** — both whiskers can extend all the way to the minimum and maximum.

**Symmetry**: Compare the two halves of the box and the two whiskers:

- Distance from Q1 to Median: $60 - 52 = 8$
- Distance from Median to Q3: $68 - 60 = 8$
- Distance from Min to Q1 (left whisker): $52 - 45 = 7$
- Distance from Q3 to Max (right whisker): $75 - 68 = 7$

Both halves of the box are the same length (8 each), and both whiskers are the same length (7 each). This tells us the distribution is **roughly symmetric** — the data is spread out fairly evenly on either side of the median.

![Boxplot from a 5-number summary](https://drolsonmi.github.io/math1040/Lesson06/images/Fig652_Solution.png)

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson06/6_5_Boxplots.html#practice)
