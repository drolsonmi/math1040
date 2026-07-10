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
<title>Solution for practice 7.1.2</title>
</head>

## 7.1 Variance - Solution for Practice 2
2. A researcher weighs a **sample** of 5 puppies from a large litter: $[8, 10, 9, 11, 12]$ pounds. Find the sample variance.

### Solution
 
Since these 5 puppies are only a sample from a larger litter (not the entire litter), we use the **sample variance** formula, which divides by $n-1$ instead of $n$:
 
$$s^2 = \frac{\sum (x-\bar{x})^2}{n-1}$$
 
**Step 1: Find the mean.**
 
$$\bar{x} = \frac{8+10+9+11+12}{5} = \frac{50}{5} = 10$$
 
**Step 2: Find each deviation $(x - \bar{x})$, then square it.**
 
| $x$ | $x-\bar{x}$ | $(x-\bar{x})^2$ |
| --- | --- | --- |
| 8  | -2 | 4 |
| 10 | 0  | 0 |
| 9  | -1 | 1 |
| 11 | 1  | 1 |
| 12 | 2  | 4 |
 
**Step 3: Add up the squared deviations.**
 
$$\sum(x-\bar{x})^2 = 4+0+1+1+4 = 10$$
 
**Step 4: Divide by $n-1$ (since this is a sample, $n-1 = 5-1 = 4$).**
 
$$s^2 = \frac{10}{4} = 2.5$$
 
The sample variance is **$2.5~pounds^2$**.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_1_Variance.html#practice)