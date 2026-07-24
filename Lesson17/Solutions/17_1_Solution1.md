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
<title>Solution for practice 17.1.1</title>
</head>

## 17.1 Sampling Distributions - Solution for Practice 1
1. A fair six-sided die is rolled one time. In a separate experiment, a fair six-sided die is rolled 40 times, and the average of those 40 rolls is recorded. Which of these two values - the single roll, or the average of 40 rolls - is more likely to land close to the population mean of 3.5? Explain your reasoning.

### Solution

The average of the 40 rolls is far more likely to land close to the population mean of 3.5.

A single roll can land on any of the six values (1, 2, 3, 4, 5, or 6) with equal probability. There is nothing pulling that single roll toward the mean - it is just as likely to come up 1 or 6 as it is to come up 3 or 4.

However, once we start averaging many rolls together, extreme values start to cancel each other out. If one roll happens to be a 6, it takes several low rolls to balance it out for the average to still be far from 3.5. As we saw in this lesson, larger samples produce sampling distributions that are more tightly clustered around the population mean - the histograms got narrower and more bell-shaped as the sample size increased from 2 dice, to 5, to 10, to 20, 30, and 50 dice.

So, the average of 40 rolls belongs to a sampling distribution with much less spread than the distribution of individual rolls, making it much more likely to be close to $\mu = 3.5$.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_1_SamplingDistributions.html#practice)
