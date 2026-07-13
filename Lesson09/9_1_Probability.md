<head>
<title>Lesson 9.1 Probability</title>
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

# Lesson 9.1 Probability
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1.1 Probability (pages 88-90)

## Lesson
Before we can calculate a probability, we need to be clear on exactly what we're measuring. A few key terms will show up throughout this entire lesson:
 
- **Event**: An action or process that produces one of several possible results. Rolling a die, flipping a coin, and drawing a card are all examples of events.
- **Outcome**: A single possible result of an event. Rolling a 5 is one outcome of the event "rolling a die."
- **Sample Space**: The complete list of every possible outcome of an event. For rolling a standard die, the sample space is $\{1, 2, 3, 4, 5, 6\}$.
### What Is a Probability?
 
A **probability** is a number that tells us how likely a particular outcome (or group of outcomes) is to occur. When every outcome in the sample space is equally likely, we calculate the **theoretical probability** of an event $A$ with the formula:
 
$$P(A) = \frac{\text{number of outcomes in } A}{\text{number of outcomes in the sample space}}$$
 
For example, suppose we roll a standard die and want to find the probability of rolling a number larger than 2:
 
- The sample space is $\{1, 2, 3, 4, 5, 6\}$, which has 6 outcomes.
- The outcomes that satisfy "larger than 2" are $\{3, 4, 5, 6\}$, which has 4 outcomes.
$$P(\text{larger than } 2) = \frac{4}{6} = \frac{2}{3} \approx 0.667 = 66.7\%$$
 
### Two Rules Every Probability Must Follow
 
1. **A probability is always between 0 and 1** (or 0% and 100%). A probability of 0 means an outcome is impossible; a probability of 1 means an outcome is certain. A probability can never be negative, and it can never be larger than 1.
$$0 \le P(A) \le 1$$
 
2. **The probabilities of every outcome in a sample space must add up to 1.** If you listed the probability of rolling each number 1 through 6 on a die, those six probabilities would sum to exactly 1 (100%), since one of those six outcomes is guaranteed to happen.
### Probability vs. Relative Frequency
 
It's worth previewing an important distinction we'll dig into further in 9.2: **theoretical probability** is calculated using the sample space (what *should* happen, assuming every outcome is equally likely), while **relative frequency** is calculated from real, observed data (what *actually* happened). If you flip a fair coin, the theoretical probability of heads is exactly $P(\text{heads}) = 0.5$, but if you actually flip that coin 20 times, you might get heads 9 times out of 20 — a relative frequency of $\frac{9}{20} = 0.45$. Both numbers are useful, but they answer slightly different questions.

<iframe width="560" height="315" src="https://www.youtube.com/embed/5KiZNdfxjYc?si=1MS2-gra4oG4SQro" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. A fair six-sided die is rolled once. Find the probability of rolling an **even number**.
    - [After solving on your own, see solution here](Solutions/9_1_Solution1.md).
2. A standard deck of 52 playing cards has 4 suits (hearts, diamonds, clubs, spades) with 13 cards in each suit. One card is drawn at random. Find the probability that the card is a **heart**.
    - [After solving on your own, see solution here](Solutions/9_1_Solution2.md).
3. A bag contains 5 red marbles, 3 blue marbles, and 2 green marbles. One marble is drawn at random. Find the probability that the marble is **blue**.
    - [After solving on your own, see solution here](Solutions/9_1_Solution3.md).
 
