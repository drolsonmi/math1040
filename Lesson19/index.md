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

# Lesson 19: Confidence Intervals with 1 Sample Proportions
Let's turn our attention to creating confidence intervals for categorical data. That means that instead of means and standard deviations, we will use proportions.

A few things to note while using proportions:

* Since we aren't working with standard deviations, we don't have to worry about whether we have a population value or not it or not. So, we will ALWAYS be using the z-score. The t-score will *not* appear at all whenever we are using proportions.
* Remember that a proportions always have a value between 0 and 1. That means that the boundaries for our confidence intervals will also be between 0 and 1.
    * If you get a confidence interval with a boundary above 1 or below 0, then something went wrong.

While interpreting categorical confidence intervals, there is an additional aspect we can add to our interpretation:
* If both of the boundaries of our confidence interval are above 0.50, then we are quite confident that we have a majority. 
* Likewise, if both of the boundaries of our confidence interval are below 0.50, then we are quite confident that we have a minority

## Quick example
Presidential elections are a great example of this. Election committees often put out surveys to see if citizens in a state will vote for a given candidate. Let's say that in Utah, a survey to determine whether citizens vote republican or not shows a 99% confidence interval of (0.65, 0.8).

Since we are 99% confident that the overall proportion of Utah citizens that vote republican is between 0.65 and 0.80 (between 65% and 80%), then we are very confident that the state will vote republican.

Next presidential election, watch the news when polls close. You'll see that they will declare Utah as republican before they count a single vote. This is because the confidence interval is so clearly in the majority.

## Outcomes
By the end of this lesson, you should be able to:
* Calculate a sample proportion ($\hat{p}$) and its complement ($\hat{q}$) from a categorical dataset
* Verify that the Central Limit Theorem applies to a proportion (random sample, $n\hat{p}\ge 10$ and $n\hat{q}\ge 10$)
* Find the critical value ($z_c$) for a given confidence level
* Calculate the margin of error for a proportion
* Construct a confidence interval for a proportion
* Interpret a confidence interval for a proportion, including whether it suggests a majority or minority

## Topics in this lecture
In this lesson, we'll learn how to find the confidence interval for categorical data using proportions.
* [19.1 Critical Values](./19_1_CriticalValues.md)
* [19.2 Confidence Intervals with 1 Sample Proportions](./19_2_ConfidenceIntervalProps.md)