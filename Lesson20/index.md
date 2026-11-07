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

# Lesson 20: Hypothesis Testing with 1 Quantitative Sample
## What is a Hypothesis Test?
So far, whenever we wanted to say something about a population, we built a __confidence interval__ — a range of values where we believe the true population parameter (a mean or a proportion) is likely to fall. A confidence interval answers the question, *"What is the true value, roughly?"*

Starting with this lesson, we ask a slightly different question: *"Is there evidence that the true value is different from some specific, claimed value?"* This is the idea behind a __hypothesis test__.

A hypothesis test starts with a claim about a population parameter — for example, a company's claim about an average, or a belief about whether that average has changed. We call this claimed value the __null value__. We then use a sample to decide whether the data give us enough evidence to doubt that claim.

Hypothesis tests and confidence intervals are two sides of the same coin. In fact, as we will see in this lesson, a confidence interval can be used to make the exact same decision as a hypothesis test. The difference is really about the __question being asked__ and how we report the result:
* A confidence interval reports a __range of plausible values__
* A hypothesis test reports a __decision__ about a specific claimed value, along with a measure of how much evidence we have for that decision

The rest of this course is built around hypothesis testing, so it's worth taking the time now to understand exactly what a hypothesis test is doing and why.

## Quick example
American mental abilities are often measured by an IQ test. The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. Suppose a random sample of 40 Snow College students has an average IQ of 106.3.

Instead of asking, "What is a range of plausible values for the true average IQ of Snow College students?" (a confidence interval question), we now ask, "Is there enough evidence to say that the true average IQ of Snow College students is *higher* than the national average of 100?" (a hypothesis test question).

To answer this, we start with the assumption that there is __no difference__ — that the true average IQ at Snow College is the same as the national average, 100. This is our null value. We then use the sample data (a sample average of 106.3) to see whether there is enough evidence to reject that assumption in favor of the claim that Snow College students score higher.

We'll use this same example throughout the rest of this lesson to walk through each piece of a hypothesis test, from writing the hypotheses to reaching a final conclusion.

## Outcomes
By the end of this lesson, you should be able to:
* Explain the purpose of a hypothesis test and how it relates to a confidence interval
* Write the null and alternate hypotheses for a given claim
* Identify a hypothesis test as left-tailed, right-tailed, or two-tailed
* Find the critical region for a hypothesis test at a given level of significance
* Calculate a test statistic and use it, together with the critical region, to make a decision
* Calculate a p-value and use it to make a decision
* Carry out a complete hypothesis test for a population mean, from hypotheses to conclusion

## Topics in this lecture
* [20.1 Hypotheses](./20_1_Hypotheses.md)
* [20.2 How Confidence Intervals fit in](./20_2_HypTestAndConfInt.md)
* [20.3 Critical Regions](./20_3_CriticalRegions.md)
* [20.4 P-values](./20_4_PValues.md)
* [20.5 Hypothesis Test with 1 Quantitative Sample](./20_5_HypTest1SampleMeans.md)