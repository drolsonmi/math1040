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

## Lesson 15: Normal Distributions

Up until this point, we have dealt with the probability distributions of discrete variables. For many categorical variables, this will be the case. These work well because we can find the probability of a specific category.

However, there are some variables that are continuous. In this case, we can't find the probability of a specific value since having an exact value is nearly impossible.

- For example, what is the probability of a person weighing exactly 170 lbs? Very small because most people at 170 lbs could be 169.95 lbs or 170.4 lbs, etc. The number of people who are exactly 170.00000000000 lbs is extremely small.

The solution then is to look instead at a range of numbers. The primary tool we'll use for this is the **Normal Distribution**. This is what we will study in this lesson.

## Quick example

- On an exam with 20 multiple choice questions, what is the probability of getting 10 questions correct?
  * This is a discrete variable. We can get exactly 9 questions correct, 10 questions correct, or 11 questions correct. We can't get 10.5 questions or 9.2 questions.
  * Because of this, we can create a probability distribution and find a probability of one category ( $P(X = 10)$ ) or a cumulative probability of a bunch of categories ( $P(X \ge 10)$ ).
- At a local ice cream shop, students get ice cream to relax after taking their exams. What is the probability that a single scoop weighs 7.0 ozs?
  * The size of each scoop varies, which means the scoops can be 6.8, 6.9, 6.97, 6.999997, 7.01, 7.2, ...
  * The probability of getting *exactly* 7.0 ozs is extremely small
  * Instead, we'll look at the probability of getting between 6.9 and 7.1 ozs.

## Lesson Objectives

By the end of this lesson, you should be able to accomplish the following:

- Distinguish between discrete and continuous distributions, and explain why the probability of an exact value is essentially zero for a continuous variable
- Describe the shape and properties of the normal distribution, and explain why area under the density curve represents probability
- Calculate the z-score of a value from a normal distribution, and use the Empirical Rule to estimate probabilities
- Use a Z-table (and technology) to find the probability associated with a given z-score or range of values
- Find the data value that corresponds to a given z-score, and use this to find values associated with a given probability or percentile

## Topics in this lecture

- [15.1 Discrete and Continuous Distributions](https://drolsonmi.github.io/math1040/Lesson15/15_1_ContinuousVars.html)
- [15.2 The Normal Distribution](https://drolsonmi.github.io/math1040/Lesson15/15_2_NormalDistributions.html)
- [15.3 Probability from a Normal Distribution](https://drolsonmi.github.io/math1040/Lesson15/15_3_ProbabilityFromNormal.html)
  * [Z-Tables](https://drolsonmi.github.io/math1040/Resources/Z-Table.pdf)
- [15.4 Finding the Z-score from a Probability](https://drolsonmi.github.io/math1040/Lesson15/15_4_FindingZScore.html)
