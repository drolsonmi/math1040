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
<title>Solution for practice 7.1.3</title>
</head>

## 7.1 Variance - Solution for Practice 3
3. Two vending machines are each timed on 5 separate fills (in seconds):
  - Machine A: $[30, 32, 31, 29, 33]$
  - Machine B: $[25, 40, 20, 35, 30]$
  - Treating each list as a sample, find the sample variance for Machine A and for Machine B. Which machine is more consistent? Explain how the variance tells you this.
{:start="3"}

### Solution
 
**Machine A**
 
Mean: $$\bar{x} = \frac{30+32+31+29+33}{5} = \frac{155}{5} = 31$$
 
| $x$ | $x-\bar{x}$ | $(x-\bar{x})^2$ |
| --- | --- | --- |
| 30 | -1 | 1 |
| 32 | 1  | 1 |
| 31 | 0  | 0 |
| 29 | -2 | 4 |
| 33 | 2  | 4 |
 
$$\sum(x-\bar{x})^2 = 1+1+0+4+4 = 10$$
 
$${s_A}^2 = \frac{10}{5-1} = \frac{10}{4} = 2.5$$
 
**Machine B**
 
Mean: $$\bar{x} = \frac{25+40+20+35+30}{5} = \frac{150}{5} = 30$$
 
| $x$ | $x-\bar{x}$ | $(x-\bar{x})^2$ |
| --- | --- | --- |
| 25 | -5  | 25  |
| 40 | 10  | 100 |
| 20 | -10 | 100 |
| 35 | 5   | 25  |
| 30 | 0   | 0   |
 
$$\sum(x-\bar{x})^2 = 25+100+100+25+0 = 250$$
 
$${s_B}^2 = \frac{250}{5-1} = \frac{250}{4} = 62.5$$
 
**Comparison**: Machine A has a sample variance of 2.5 seconds², while Machine B has a sample variance of 62.5 seconds² — 25 times larger. Since variance measures how spread out the values are around the mean, the much smaller variance for Machine A tells us its fill times stay much closer to its average of 31 seconds. Machine B's fill times swing much more widely around its average of 30 seconds.
 
**Machine A is more consistent**, because a smaller variance means the data values are clustered more tightly around the mean, with less variability from fill to fill.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_1_Variance.html#practice)