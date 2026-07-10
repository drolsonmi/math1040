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
<title>Solution for practice 7.3.2</title>
</head>

## 7.3 The Z-Score - Solution for Practice 2
2. Sally scores 88 on Test A, where the mean was 80 and the standard deviation was 4. Tom scores 91 on Test B, a completely different test, where the mean was 85 and the standard deviation was 2. Find each student's z-score, and determine who performed better relative to their own test.

### Solution
Since Sally and Tom took two different tests with different means and different standard deviations, we can't compare their raw scores of 88 and 91 directly. Converting each score to a z-score puts both students on the same standardized scale.
 
**Sally (Test A)**: $x = 88$, $\bar{x} = 80$, $s = 4$
 
$$z_{Sally} = \frac{88-80}{4} = \frac{8}{4} = 2$$
 
**Tom (Test B)**: $x = 91$, $\bar{x} = 85$, $s = 2$
 
$$z_{Tom} = \frac{91-85}{2} = \frac{6}{2} = 3$$
 
**Comparison**: Sally's score is 2 standard deviations above her test's mean, while Tom's score is 3 standard deviations above his test's mean. Even though 91 is a higher raw score than 88, **Tom performed better relative to his own test**, because his score is farther above the average (in standard deviation units) than Sally's.
 
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson07/7_3_ZScore.html#practice)