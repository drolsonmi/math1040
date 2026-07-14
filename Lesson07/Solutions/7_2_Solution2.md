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
<title>Solution for practice 7.2.2</title>
</head>

## 7.2 Standard Deviation - Solution for Practice 2
2. A researcher records the reaction times (in tenths of a second) of a **sample** of 6 volunteers: $[5, 7, 9, 9, 11, 13]$. Find the sample standard deviation.
{:start="2"}

### Solution
 
Since these 6 volunteers are only a sample (not the entire population being studied), we use the **sample standard deviation** formula, which divides by $n-1$ instead of $n$:
 
$$s = \sqrt{\frac{\sum(x-\bar{x})^2}{n-1}}$$
 
**Step 1: Find the mean.**
 
$$\bar{x} = \frac{5+7+9+9+11+13}{6} = \frac{54}{6} = 9$$
 
**Step 2: Find each deviation $(x - \bar{x})$, then square it.**
 
| $x$ | $x-\bar{x}$ | $(x-\bar{x})^2$ |
| --- | --- | --- |
| 5  | -4 | 16 |
| 7  | -2 | 4  |
| 9  | 0  | 0  |
| 9  | 0  | 0  |
| 11 | 2  | 4  |
| 13 | 4  | 16 |
 
**Step 3: Add up the squared deviations, then divide by $n-1$ to get the variance.**
 
$$\sum(x-\bar{x})^2 = 16+4+0+0+4+16 = 40$$
 
$$s^2 = \frac{40}{6-1} = \frac{40}{5} = 8$$
 
**Step 4: Take the square root of the variance to get the standard deviation.**
 
$$s = \sqrt{8} \approx 2.83$$
 
The sample standard deviation is approximately **2.83 tenths of a second** (about 0.283 seconds).
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_2_StandardDeviation.html#practice)