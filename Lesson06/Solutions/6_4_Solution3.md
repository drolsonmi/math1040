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
<title>Solution for practice 6.4.3</title>
</head>

## 6.4 Quartiles - Solution for Practice 3

3. A dataset has the 5-number summary: Min = 10, Q1 = 25, Median = 40, Q3 = 58, Max = 90.
  - What percentile does Q1 correspond to?
  - What is the IQR?
  - What proportion of the data lies between Q1 and Q3?
{:start="3"}

### Solution

**Percentile for Q1**: The 1st quartile separates the lowest quarter (25%) of the data from the rest, so Q1 corresponds to the **25th percentile**.

**IQR**: The interquartile range is the distance between Q1 and Q3:

$$IQR = Q_3 - Q_1 = 58 - 25 = 33$$

**Proportion between Q1 and Q3**: Q1 marks the boundary of the lowest 25% of the data, and Q3 marks the boundary of the lowest 75% of the data. So the region between them contains the middle 50% of the data — that is, a proportion of **0.50 (50%)**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson06/6_4_Quartiles.html#practice)
