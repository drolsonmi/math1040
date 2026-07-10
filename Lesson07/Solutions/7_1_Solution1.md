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
<title>Solution for practice 7.1.1</title>
</head>

## 7.1 Variance - Solution for Practice 1
1. The ages of all 6 employees at a small office are: $[24, 28, 22, 30, 26, 26]$. Since this is every employee at the office, treat this as a **population**. Find the population variance.

### Solution
 
Since this dataset includes every employee at the office (not just a sample of them), we use the **population variance** formula:
 
$$\sigma^2 = \frac{\sum (x-\mu)^2}{n}$$
 
**Step 1: Find the mean.**
 
$$\mu = \frac{24+28+22+30+26+26}{6} = \frac{156}{6} = 26$$
 
**Step 2: Find each deviation $(x - \mu)$, then square it.**
 
| $x$ | $x-\mu$ | $(x-\mu)^2$ |
| --- | --- | --- |
| 24 | -2 | 4 |
| 28 | 2 | 4 |
| 22 | -4 | 16 |
| 30 | 4 | 16 |
| 26 | 0 | 0 |
| 26 | 0 | 0 |
 
**Step 3: Add up the squared deviations.**
 
$$\sum(x-\mu)^2 = 4+4+16+16+0+0 = 40$$
 
**Step 4: Divide by $n$ (since this is a population).**
 
$$\sigma^2 = \frac{40}{6} \approx 6.67$$
 
The population variance is approximately **6.67 years²**.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_1_Variance.html#practice)