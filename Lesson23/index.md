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

# Lesson 23: Hypothesis Testing with 2 Independent Samples (Proportions)

## Overview
Lesson 22 extended hypothesis testing to compare two independent means. This lesson does the same thing for **categorical** data — comparing two independent **proportions** ($p_1$ and $p_2$) instead of a single proportion to a claimed value.

The overall process should feel very familiar by now: verify the conditions, state hypotheses, calculate a test statistic (always a z-score, just as it was for a single proportion in Lesson 21), find the critical value and/or p-value, and make a decision. The only real difference is that we're now comparing two sample proportions to each other, and the standard error formula accounts for both samples at once.

As with Lesson 22, everything here assumes the two samples are **independent** (see Lesson 22.1 for a reminder of what that means).

## Outcomes
By the end of this lesson, you should be able to:
* Write the null and alternate hypotheses for comparing two population proportions
* Verify the conditions required to compare two independent proportions, including the success-failure condition using a pooled proportion
* Construct and interpret a confidence interval for the difference of two proportions ($p_1 - p_2$)
* Carry out a complete hypothesis test comparing two independent sample proportions, from hypotheses to conclusion
* Perform each of these calculations using a TI-83/84 calculator, Excel, and Desmos

## Topics in this lesson
* [23.1 Hypotheses of 2 Independent Categorical Samples](./23_1_Hypotheses.md)
* [23.2 Confidence Intervals for 2 Independent Categorical Samples](./23_2_ConfidenceIntervals.md)
* [23.3 Hypothesis Test of 2 Independent Categorical Samples](./23_3_HypothesisTest.md)
