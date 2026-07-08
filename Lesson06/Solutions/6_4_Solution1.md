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
<title>Solution for practice 6.4.1</title>
</head>

## 6.4 Quartiles - Solution for Practice 1

1. Find the 5-number summary of the following dataset: \[2, 4, 6, 8, 10, 12, 14, 16, 18\]

### Solution

The dataset is already ordered and has \(n = 9\) values (odd).

**Minimum**: 2
**Maximum**: 18

**Median**: with 9 values, the median is the middle (5th) value:

$$2, 4, 6, 8, \mathbf{10}, 12, 14, 16, 18$$

Median = **10**

**Q1**: the median of the lower half, not including the overall median: \[2, 4, 6, 8\]

$$Q_1 = \dfrac{4+6}{2} = 5$$

**Q3**: the median of the upper half, not including the overall median: \[12, 14, 16, 18\]

$$Q_3 = \dfrac{14+16}{2} = 15$$

**5-number summary**:

| Minimum | Q1 | Median | Q3 | Maximum |
| ------- | -- | ------ | -- | ------- |
| 2       | 5  | 10     | 15 | 18      |

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson06/6_4_Quartiles.html#practice)
