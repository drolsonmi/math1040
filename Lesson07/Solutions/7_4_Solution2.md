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
<title>Solution for practice 7.4.2</title>
</head>

## 7.4 The Empirical Rule - Solution for Practice 2
2. Using the same light bulb data (mean = 1200 hours, standard deviation = 50 hours), estimate the percentage of light bulbs that last **less than 1100 hours**.
{:start="2"}

### Solution
 
**Step 1: Figure out how many standard deviations 1100 is from the mean.**
 
$$1200 - 1100 = 100 = 2 \times 50$$
 
So 1100 hours is exactly **2 standard deviations below the mean**.
 
**Step 2: Use the Empirical Rule.** About 95% of the data falls within 2 standard deviations of the mean, which means the remaining data is split evenly between the two tails **beyond** 2 standard deviations:
 
$$\frac{100\% - 95\%}{2} = \frac{5\%}{2} = 2.5\%$$
 
Since we want the tail *below* the mean (values less than 1100 hours), this is exactly the lower tail we just found.
 
About **2.5% of the light bulbs last less than 1100 hours**.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_4_EmpiricalRule.html#practice)