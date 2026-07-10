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
<title>Solution for practice 7.2.1</title>
</head>

## 7.2 Standard Deviation - Solution for Practice 1
1. A teacher records the ages of all 5 students in a small tutoring group: $[10, 12, 14, 16, 18]$. Since this is every student in the group, treat this as a **population**. Find the population standard deviation.

### Solution
 
Since this dataset includes every student in the group, we use the **population standard deviation** formula:
 
$$\sigma = \sqrt{\frac{\sum(x-\mu)^2}{n}}$$
 
**Step 1: Find the mean.**
 
$$\mu = \frac{10+12+14+16+18}{5} = \frac{70}{5} = 14$$
 
**Step 2: Find each deviation $(x - \mu)$, then square it.**
 
| $x$ | $x-\mu$ | $(x-\mu)^2$ |
| --- | --- | --- |
| 10 | -4 | 16 |
| 12 | -2 | 4  |
| 14 | 0  | 0  |
| 16 | 2  | 4  |
| 18 | 4  | 16 |
 
**Step 3: Add up the squared deviations, then divide by $n$ to get the variance.**
 
$$\sum(x-\mu)^2 = 16+4+0+4+16 = 40$$
 
$$\sigma^2 = \frac{40}{5} = 8$$
 
**Step 4: Take the square root of the variance to get the standard deviation.**
 
$$\sigma = \sqrt{8} \approx 2.83$$
 
The population standard deviation is approximately **2.83 years**.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_2_StandardDeviation.html#practice)