<head>
<title>Lesson 15.1 Discrete and Continuous Distributions</title>
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

# Lesson 15.1 Discrete and Continuous Distributions
## Reading

Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)

- 3.6 Continuous distributions (pages 125-127)

## Lesson

Back in [Lesson 12](../Lesson12/index.html), we built probability distributions for **discrete** variables — variables that can only take on a countable list of values (0, 1, 2, 3, ...). For a discrete variable, it makes sense to ask for the probability of *one specific value*, like $P(X = 3)$, because there are only so many possible values, and each one takes up a real "chunk" of the probability.

A **continuous** variable is different. It can take on *any* value within a range, including decimals with infinitely many digits — things like height, weight, time, and temperature. Because there are infinitely many possible values in any interval, no single value takes up any measurable share of the probability. This leads to a strange but important fact:

$$P(X = a) = 0 \text{ for any exact value } a \text{, when } X \text{ is continuous}$$

For example, asking "what is the probability that a randomly selected adult weighs *exactly* 170.00000... lbs?" doesn't really make sense — nobody weighs an exact, infinitely precise value. What we *can* ask, and what actually matters in practice, is the probability that the adult's weight falls in a **range**, like between 165 and 175 lbs.

### Density Curves

Instead of a probability distribution table or histogram, continuous variables are described using a **density curve** — a smooth curve where:

- The curve is always on or above the x-axis (no negative probabilities)
- The **total area** underneath the entire curve equals exactly **1** (100% of all outcomes)
- The probability of the variable falling between any two values $a$ and $b$ is equal to the **area under the curve** between $a$ and $b$

This last point is the key idea we'll build on for the rest of this lesson: **area under a density curve = probability**. Many different shapes of density curves exist, but the one we will focus on for the remainder of this lesson (and the next) is the most common and useful one in statistics: the **Normal Distribution**.

<iframe width="560" height="315" src="https://www.youtube.com/embed/CAbbBJsAwi0?si=uuIRL6BlFdSbwf36" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice

For each variable described below, state whether it is discrete or continuous, and briefly explain why.

1. The number of siblings a randomly selected student has.
  - [After solving on your own, see solution here](./Solutions/15_1_Solution1.html)
2. The amount of rainfall (in inches) a city receives during the month of March.
  - [After solving on your own, see solution here](./Solutions/15_1_Solution2.html)
3. Explain why it doesn't make sense to ask for the probability that a randomly selected adult weighs *exactly* 150 lbs, and describe how we would instead find a meaningful probability about that adult's weight.
  - [After solving on your own, see solution here](./Solutions/15_1_Solution3.html)
