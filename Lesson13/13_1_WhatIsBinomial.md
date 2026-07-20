<head>
<title>Lesson 13.1 What is a Binomial Distribution?</title>
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

# Lesson 13.1 What is a Binomial Distribution?
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 4.3 Binomial distribution (pages 149-158)

## Lesson
Many random processes boil down to repeating the same simple trial over and over, where each trial has only two possible outcomes: __success__ or __failure__. Think of flipping a coin, checking whether a product coming off an assembly line is defective, or asking people whether they plan to vote. A distribution built out of many repeated trials like this is called a __binomial distribution__.

### The Four Requirements of a Binomial Experiment

A random process is a __binomial experiment__ only if it satisfies all four of the following conditions:

1. __Fixed number of trials.__ The number of trials, $n$, is set in advance and doesn't change.
2. __Two outcomes per trial.__ Each trial results in one of exactly two outcomes, which we label __success__ and __failure__.
3. __Constant probability of success.__ The probability of success, $p$, is the same on every trial. (The probability of failure is then $q = 1-p$.)
4. __Independent trials.__ The outcome of one trial does not affect the outcome of any other trial.

If even one of these conditions fails, the process is *not* binomial, and the tools in this lesson won't apply.

### Binomial Notation

We use a standard set of symbols to describe a binomial experiment:

$$\begin{align*}
  n &= \text{number of trials} \\
  p &= \text{probability of success on a single trial} \\
  q = 1-p &= \text{probability of failure on a single trial} \\
  r &= \text{number of successes we are interested in } (r = 0, 1, 2, \dots, n)
\end{align*}$$

For example, suppose 30% of customers who enter a store make a purchase, and we watch 8 randomly chosen, independent customers. This is binomial with $n=8$ and $p=0.30$. If we want the probability that exactly 3 of them make a purchase, then $x=3$.

### A Word of Caution: Independence and "Without Replacement"

Condition 4 (independence) is the one students most often overlook. If we are drawing from a small population *without replacement*, the probability of success can change from trial to trial, which breaks independence, and the process is technically **not** binomial. In practice, if the population is very large compared to the sample (a common rule of thumb is that the sample is less than 10% of the population), the change in probability from trial to trial is so small that we treat the process as approximately binomial anyway.

<iframe width="560" height="315" src="https://www.youtube.com/embed/J8jNoF-K8E8?si=Vv3nZ54nTOoOLZ0d" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
For each scenario, decide whether the process describes a binomial experiment. If it does, identify $n$, $p$, and $q$. If it does not, explain which requirement is not met.

1. A fair coin is flipped 10 times, and we count the number of heads.
  - [After solving on your own, see solution here](./Solutions/13_1_Solution1.html)
2. A bag contains 4 red marbles and 2 blue marbles. Three marbles are drawn **without replacement**, and we count the number of red marbles drawn.
  - [After solving on your own, see solution here](./Solutions/13_1_Solution2.html)
3. Historically, 8% of emails sent by a marketing company are marked as spam by the recipient's inbox. The company sends a new campaign to 500 independent recipients, and we count how many mark it as spam.
  - [After solving on your own, see solution here](./Solutions/13_1_Solution3.html)
4. A teacher calls on students **one at a time, without replacement**, from a class of 25 students to answer questions until she has called on 5 students, and records how many of the 5 are wearing glasses.
  - [After solving on your own, see solution here](./Solutions/13_1_Solution4.html)
