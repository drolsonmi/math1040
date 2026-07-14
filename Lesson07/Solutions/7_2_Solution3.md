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
<title>Solution for practice 7.2.3</title>
</head>

## 7.2 Standard Deviation - Solution for Practice 3
3. Two classes take the same 5-question quiz. A sample of scores from each class is recorded:
{:start="3"}
  - Class A: $[78, 82, 85, 80, 90]$
  - Class B: $[83, 84, 82, 83, 83]$
  - Find the sample standard deviation for each class. Both classes have the same mean — what does the standard deviation tell you about how the two classes differ?

### Solution
 
**Class A**
 
Mean: $$\bar{x} = \frac{78+82+85+80+90}{5} = \frac{415}{5} = 83$$
 
| $x$ | $x-\bar{x}$ | $(x-\bar{x})^2$ |
| --- | --- | --- |
| 78 | -5 | 25 |
| 82 | -1 | 1  |
| 85 | 2  | 4  |
| 80 | -3 | 9  |
| 90 | 7  | 49 |
 
$$\sum(x-\bar{x})^2 = 25+1+4+9+49 = 88$$
 
$$s^2_A = \frac{88}{5-1} = \frac{88}{4} = 22$$
 
$$s_A = \sqrt{22} \approx 4.69$$
 
**Class B**
 
Mean: $$\bar{x} = \frac{83+84+82+83+83}{5} = \frac{415}{5} = 83$$
 
| $x$ | $x-\bar{x}$ | $(x-\bar{x})^2$ |
| --- | --- | --- |
| 83 | 0  | 0 |
| 84 | 1  | 1 |
| 82 | -1 | 1 |
| 83 | 0  | 0 |
| 83 | 0  | 0 |
 
$$\sum(x-\bar{x})^2 = 0+1+1+0+0 = 2$$
 
$$s^2_B = \frac{2}{5-1} = \frac{2}{4} = 0.5$$
 
$$s_B = \sqrt{0.5} \approx 0.71$$
 
**Interpretation**: Both classes are centered at the same mean score of 83, so on average, the two classes performed identically. However, Class A has a standard deviation of about 4.69 points, while Class B has a standard deviation of only about 0.71 points. This tells us that Class A's scores are typically spread about 4.69 points away from the mean, while Class B's scores stay tightly clustered within about 0.71 points of the mean. In other words, even though both classes averaged the same score, **Class A had much more variability in performance** (a wider mix of high and low scores), while **Class B was far more consistent**.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_2_StandardDeviation.html#practice)