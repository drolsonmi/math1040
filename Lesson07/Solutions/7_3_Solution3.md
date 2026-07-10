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
<title>Solution for practice 7.3.3</title>
</head>

## 7.3 The Z-Score - Solution for Practice 3
3. A dataset has a mean of 50 and a standard deviation of 8. What data value corresponds to a z-score of $-1.5$?

### Solution
This problem gives us the z-score and asks us to work backward to find the original data value $x$. Start with the z-score formula and solve for $x$:
 
$$z = \frac{x-\bar{x}}{s} \quad\Longrightarrow\quad x = \bar{x} + z\cdot s$$
 
Here, $\bar{x} = 50$, $s = 8$, and $z = -1.5$.
 
$$x = 50 + (-1.5)(8) = 50 - 12 = 38$$
 
The data value is **38**. This makes sense: a negative z-score means the value should fall *below* the mean, and 38 is indeed 1.5 standard deviations below the mean of 50.

- The figure on the left is a normal distribution with a mean of 50 and a standard deviation of 8. The dotted line indicates the value $x = 38$.
- The figure on the right is a standardized normal distribution. The dotted line indicates the z-score $z = -1.5$.
- Notice how they are essentially identical. The z-score represents the original value on the standardized normal distribution.

![Comparison of normal and standardized normal distributions](../images/Fig733_Solution1.png)

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_3_ZScore.html#practice)