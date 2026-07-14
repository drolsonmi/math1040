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
<title>Solution for practice 7.4.3</title>
</head>

## 7.4 The Empirical Rule - Solution for Practice 3
3. Using the same light bulb data (mean = 1200 hours, standard deviation = 50 hours), estimate the percentage of light bulbs that last **between 1250 and 1300 hours**.
{:start="3"}

### Solution
 
**Step 1: Locate 1250 and 1300 in terms of standard deviations from the mean.**
 
$$1250 - 1200 = 50 = 1 \times 50 \quad\Rightarrow\quad 1250 \text{ is } 1 \text{ standard deviation above the mean}$$
 
$$1300 - 1200 = 100 = 2 \times 50 \quad\Rightarrow\quad 1300 \text{ is } 2 \text{ standard deviations above the mean}$$
 
So we need the percentage of data that falls **between 1 and 2 standard deviations above the mean**.
 
**Step 2: Use the Empirical Rule percentages for 1 and 2 standard deviations.**
 
- Within 1 standard deviation of the mean: 68%
- Within 2 standard deviations of the mean: 95%

**Step 3: Subtract to isolate the band between 1 and 2 standard deviations (both sides combined), then divide by 2 for just the upper side**, since the normal distribution is symmetric:
 
$$\frac{95\% - 68\%}{2} = \frac{27\%}{2} = 13.5\%$$
 
About **13.5% of the light bulbs last between 1250 and 1300 hours**.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_4_EmpiricalRule.html#practice)