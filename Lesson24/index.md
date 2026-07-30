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

# Lesson 24: Hypothesis Testing with 2 Dependent Samples (Means)

## Overview
Lesson 22 covered hypothesis tests comparing two **independent** samples. This lesson covers the other case from Lesson 22.1: **dependent (paired)** samples, where each observation in one group is matched to exactly one observation in the other group (before/after measurements, matched pairs, twins, left hand/right hand, and so on).

The good news is that paired data doesn't require any new formulas. Instead, we use a clever shortcut: subtract each pair to create a single new variable, the **difference** ($d$). Once we have that one variable, comparing two dependent samples becomes exactly the same problem as Lesson 20 — a **one-sample** hypothesis test, just applied to $d$ instead of $x$, with a null value of 0.

This lesson walks through that shortcut, then reuses everything you already know from Lesson 20 (hypotheses, confidence intervals, and the five-step hypothesis test) to work with paired data.

## Outcomes
By the end of this lesson, you should be able to:
* Recognize when two samples are dependent (paired) and set up the difference variable, $d$
* Calculate $\bar{d}$ and $s_d$ from paired data
* Write the null and alternate hypotheses for a test of paired differences, and verify the required conditions
* Construct and interpret a confidence interval for the mean difference, $\mu_d$
* Carry out a complete hypothesis test for paired data, from hypotheses to conclusion
* Perform each of these calculations using a TI-83/84 calculator, Excel, and Desmos

## Topics in this lesson
* [24.1 Reminder of Dependent Samples & the Difference Variable](24_1_DifferenceVariable.md)
* [24.2 Hypotheses for Paired Data](24_2_Hypotheses.md)
* [24.3 Confidence Interval for the Mean Difference](24_3_ConfidenceIntervals.md)
* [24.4 Hypothesis Test for the Mean Difference](24_4_HypothesisTest.md)
