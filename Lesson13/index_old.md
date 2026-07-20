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

## Lesson 13 Binomial Distributions
In [lesson 12](../Lesson12/index.md), we learned what a probability distribution is and how to find the expected value of a random variable. In lesson 13, we will study one of the most common and useful probability distributions: the __binomial distribution__.

A binomial distribution shows up any time we repeat the same yes/no trial over and over — flipping a coin, checking whether a part is defective, asking someone if they support a proposal — and we want to know the probability of getting a certain number of "successes." Before we get there, we'll take a short detour back to lesson 10 to review "OR" probabilities, since that idea turns out to be exactly what we need to combine binomial probabilities together.

After reviewing "OR" probabilities, we will learn the binomial probability formula and use it to find the probability of getting *exactly* a certain number of successes. Then we will build a full binomial probability distribution and use it to find the probability of getting successes *within a range* of values.

## Lesson Objectives

By the end of this lesson, you should be able to accomplish the following:

- Apply the "OR" (addition) rule to combine mutually exclusive probabilities
- Recognize whether a situation qualifies as a binomial experiment
- Calculate the probability of exactly $k$ successes in $n$ trials using the binomial probability formula
- Build a binomial probability distribution table for a given $n$ and $p$
- Calculate the probability of a range of outcomes (e.g., "3, 4, or 5 successes") using a binomial probability distribution
- Use a TI-83/84, Excel, and Desmos to calculate binomial probabilities

## Topics in this lecture
- [13.1 Review of "OR" Probabilities](./13_1_ORProbabilities.md)
- [13.2 Binomial Probabilities](./13_2_BinomialProbabilities.md)
- [13.3 Binomial Probability Distribution](./13_3_BinomialDistribution.md)
