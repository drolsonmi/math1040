<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 15: Normal Distributions
Up until this point, we have dealt with the probability distributions of discrete variables. For many categorical variables, this will be the case. These work well because we can find the probabilty of a specific category.

However, there are some variables that are continuous. In this case, we can't find the probability of a specific value since having an exact value is nearly impossible.
* For example, what is the probability of a person weighing exactly 170 lbs? Very small because most people at 170 lbs could be 169.95 lbs or 170.4 lbs, etc. The number of people who are exactly 170.00000000000 lbs is extremely small.

The solution then is to look instead at a range of numbers. The primary tool we'll use for this is the __Normal Distribution__. This is what we will study in this lesson.

## Quick example
* On an exam with 20 multiple choice questions, what is the probability of getting 10 questions correct?
  * This is a discrete variable. We can get exactly 9 questions correct, 10 questions correct, or 11 questions correct. We can't get 10.5 questions or 9.2 questions.
  * Because of this, we can create a probability distribution and find a probability of one category ( $$P(X = 10)$$ ) or a cumulative probability of a bunch of categories ( $$P(X \ge 10)$$ ).

* At a local ice cream shop, students get ice cream to relax after taking their exams. What is the probability that a single scoop weighs 7.0 ozs?
  * The size of each scoop varies, which means the scoops can be 6.8, 6.9, 6.97, 6.999997, 7.01, 7.2, ...
  * The probability of getting *exactly* 7.0 ozs is extremely small
  * Instead, we'll look at the probability of getting between 6.9 and 7.1 ozs.

## Topics in this lecture
* [15.1 Discrete and Continuous Variables](./15_1_ContinuousVars.md)
* [15.2 The Normal Distribution](./15_2_NormalDistributions.md)
* [15.3 Probability from a Normal Distribution](./15_3_ProbabilityFromNormal.md)
  * [Z-Tables](../Resources/Z-Table.pdf)
* [15.4 Finding the Z-score from a Probability](./15_4_FindingZScore.md)