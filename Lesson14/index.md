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

## Lesson 14 More on Binomial Distributions
In [lesson 13](../Lesson13/index.html), we learned how to recognize a binomial experiment and how to find the probability of __exactly__ $x$ successes. Often, though, we don't just care about one exact outcome — we care about a *range* of outcomes. What's the probability of getting *at least* 3 successes? *At most* 7? *Between* 2 and 5?

To answer these kinds of questions, we first need to revisit "OR" probabilities from [lesson 10](../Lesson10/index.html), since finding the probability of a range of outcomes means adding together the probabilities of several individual outcomes. From there, we'll generalize the idea to any discrete probability distribution, and finally apply it specifically to the binomial distribution, where technology makes these calculations fast.

## Lesson Objectives

By the end of this lesson, you should be able to accomplish the following:

- Apply the addition rule for "OR" probabilities of mutually exclusive events
- Calculate a cumulative probability (at least, at most, or between) from any discrete probability distribution by adding individual probabilities
- Calculate cumulative binomial probabilities by hand and with technology

## Topics in this lecture
- [14.1 Review of OR Probabilities](./14_1_ORProbabilities.md)
- [14.2 Cumulative Probabilities from any Discrete Probability Distribution](./14_2_CumulativeProbabilities.md)
- [14.3 Cumulative Binomial Probabilities](./14_3_CumulativeBinomialProbabilities.md)
