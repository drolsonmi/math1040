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
</head>

# Lesson 25: Hypothesis Testing with Correlation

## Overview
Earlier in this course, we calculated the correlation coefficient ($$r$$) to describe the strength and direction of a linear relationship between two quantitative variables. But $$r$$ is just a sample statistic — like $$\bar{x}$$ or $$\hat{p}$$, it's our best estimate of something we can't observe directly: the true population correlation, $$\rho$$.

This lesson asks a familiar question in a new setting: is the relationship we see in our sample strong enough to conclude there's a real linear relationship in the population, or could it just be due to chance? The good news is that by this point in the course, you already know the whole process. A correlation test uses the exact same five-step framework as every other hypothesis test we've covered — the only new pieces are the hypotheses (written in terms of $$\rho$$) and a new test statistic formula, which technology will typically calculate for you.

This is a short, focused lesson. The goal isn't to dive deeply into the theory behind correlation inference, but to make sure you can recognize a correlation hypothesis test, set it up correctly, and carry it out using a calculator, Excel, or Desmos.

## Objectives
By the end of this lesson, you should be able to:
* Distinguish between the sample correlation ($$r$$) and the population correlation ($$\rho$$)
* Write the null and alternate hypotheses for a test of correlation, and identify the test as left-tailed, right-tailed, or two-tailed
* Verify the conditions required to test a correlation
* Calculate the test statistic for a correlation test (or obtain it from technology)
* Carry out a complete hypothesis test for a correlation coefficient, from hypotheses to conclusion
* Perform this test using a TI-83/84 calculator, Excel, and Desmos

## Topics in this lesson
* [25.1 Hypotheses for a Correlation Test](25_1_Hypotheses.md)
* [25.2 Testing the Correlation Coefficient](25_2_TestingCorrelation.md)
