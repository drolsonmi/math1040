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
<title>Solution for practice 6.3.2</title>
</head>

## 6.3 Median - Solution for Practice 2

2. Find the median of the following dataset: \[8, 3, 12, 7, 15, 10\]
{:start="2"}

### Solution

First, order the dataset from smallest to largest:

$$[3, 7, 8, 10, 12, 15]$$

Since there are 6 values (an even number), there is no single middle value. The median is the average of the two middle values (the 3rd and 4th values):

$$[3, 7, \mathbf{8}, \mathbf{10}, 12, 15]$$

$$\text{Median} = \dfrac{8+10}{2} = \dfrac{18}{2} = 9$$

The median is **9**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson06/6_3_Median.html#practice)
