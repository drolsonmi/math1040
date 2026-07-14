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
<title>Solution for practice 6.4.2</title>
</head>

## 6.4 Quartiles - Solution for Practice 2

2. Find the 5-number summary of the following dataset: \[5, 7, 9, 12, 15, 18, 20, 22\]
{:start="2"}

### Solution

The dataset is already ordered and has \(n = 8\) values (even).

**Minimum**: 5
**Maximum**: 22

**Median**: with 8 values, the median is the average of the two middle (4th and 5th) values:

$$5, 7, 9, \mathbf{12}, \mathbf{15}, 18, 20, 22$$

$$\text{Median} = \dfrac{12+15}{2} = 13.5$$

**Q1**: the median of the lower half: \[5, 7, 9, 12\]

$$Q_1 = \dfrac{7+9}{2} = 8$$

**Q3**: the median of the upper half: \[15, 18, 20, 22\]

$$Q_3 = \dfrac{18+20}{2} = 19$$

**5-number summary**:

| Minimum | Q1 | Median | Q3 | Maximum |
| ------- | -- | ------ | -- | ------- |
| 5       | 8  | 13.5   | 19 | 22      |

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson06/6_4_Quartiles.html#practice)
