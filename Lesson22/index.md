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

# Lesson 22: Hypothesis Testing with 2 Independent Samples (Means)

## Overview
So far, every confidence interval and hypothesis test we've built has compared a single sample to a claimed value ($\mu_0$ or $p_0$). Many real questions instead ask us to compare **two groups** to each other: Do two teaching methods lead to different average scores? Does one fertilizer produce taller plants than another? Is the average commute time on one bus route shorter than another?

This lesson extends everything we've learned about hypothesis testing and confidence intervals to the case of **two independent samples** with **quantitative** data. The overall process is the same five steps we used in Lesson 20 — verify the conditions, state hypotheses, find the test statistic, find the critical region/p-value, and make a decision — but now we are comparing two means ($\mu_1$ and $\mu_2$) instead of one mean to a claim.

## Outcomes
By the end of this lesson, you should be able to:
* Distinguish between independent samples and dependent (paired) samples
* Write the null and alternate hypotheses for comparing two population means
* Verify the conditions required to compare two independent samples
* Construct and interpret a confidence interval for the difference of two means ($\mu_1 - \mu_2$)
* Carry out a complete hypothesis test comparing two independent sample means, from hypotheses to conclusion
* Perform each of these calculations using a TI-83/84 calculator, Excel, and Desmos

## Topics in this lesson
* [22.1 Reminder of Dependent vs. Independent Samples](./22_1_DependentVsIndependent.md)
* [22.2 Hypotheses of 2 Independent Samples](./22_2_Hypotheses.md)
* [22.3 Confidence Intervals for 2 Independent Samples](./22_3_ConfidenceIntervals.md)
* [22.4 Hypothesis Test of 2 Independent Samples](./22_4_HypothesisTest.md)
