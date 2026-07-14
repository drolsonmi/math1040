<head>
<title>Lesson 13.2 Binomial Probabilities</title>
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

# Lesson 13.2 Binomial Probabilities
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 4.3 Binomial distribution (pages 149-158)

## Lesson
A __binomial experiment__ is a specific type of repeated trial that shows up constantly in statistics. An experiment qualifies as binomial if it meets **all four** of the following conditions:

1. There is a **fixed number of trials**, $n$.
2. Each trial has only **two possible outcomes**: "success" or "failure."
3. The **probability of success**, $p$, is the **same on every trial**.
4. The trials are **independent** of one another (the outcome of one trial doesn't affect another).

Think of flipping a coin 10 times and counting how many land on heads, or surveying 50 people and counting how many support a new policy. Both fit this pattern.

### The Binomial Probability Formula

If a binomial experiment has $n$ trials, each with probability of success $p$, then the probability of getting **exactly** $k$ successes is:

$$P(X=k) = \binom{n}{k}p^k(1-p)^{n-k}\tag{Binomial Probability Formula}$$

Let's break this formula down piece by piece:

- $\binom{n}{k} = \dfrac{n!}{k!(n-k)!}$ is the **combination** from lesson 11 — it counts the number of different *orders* in which the $k$ successes could occur among the $n$ trials.
- $p^k$ is the probability that all $k$ of the successes happen, since the trials are independent (recall the "AND" rule from lesson 10: independent probabilities multiply).
- $(1-p)^{n-k}$ is the probability that the remaining $n-k$ trials are all failures.

Here's the connection back to lesson 13.1: each specific *order* of $k$ successes and $n-k$ failures is equally likely, and has probability $p^k(1-p)^{n-k}$. Since there are $\binom{n}{k}$ such orders, and getting the successes in *this* order or *that* order are mutually exclusive outcomes, we **add** the probability $p^k(1-p)^{n-k}$ to itself $\binom{n}{k}$ times — which is the same as multiplying by $\binom{n}{k}$.

### Example

Suppose 30% of customers at a coffee shop order a specialty drink. If 5 customers are selected at random, what is the probability that exactly 2 of them ordered a specialty drink?

Here, $n=5$, $p=0.3$, and we want $k=2$.

$$P(X=2) = \binom{5}{2}(0.3)^2(0.7)^3$$

$$P(X=2) = 10 \times 0.09 \times 0.343 = 0.3087$$

There is about a **30.9% chance** that exactly 2 of the 5 customers ordered a specialty drink.

<!-- Insert lesson video here -->

## Practice
1. A fair coin is flipped 8 times. What is the probability of getting exactly 5 heads?
  - [After solving on your own, see solution here](./Solutions/13_2_Solution1.html)
2. A multiple-choice quiz has 10 questions, each with 4 answer choices. A student guesses randomly on every question. What is the probability that the student gets exactly 3 questions correct?
  - [After solving on your own, see solution here](./Solutions/13_2_Solution2.html)
3. Historically, 85% of flights at a small airport depart on time. If 6 flights are selected at random, what is the probability that exactly 4 of them departed on time?
  - [After solving on your own, see solution here](./Solutions/13_2_Solution3.html)

## Technology

### TI-83/84
The calculator's binomial probability function finds $P(X=k)$ directly, without needing to compute the combination and powers by hand.

1. Press **2ND**, then **VARS** to open the **DISTR** (distributions) menu.
2. Scroll down and select **binompdf(** (binomial probability density function).
3. Enter the three values, separated by commas: `binompdf(n, p, k)`
  - $n$ = number of trials
  - $p$ = probability of success
  - $k$ = number of successes you want the probability of
4. Press **ENTER** to calculate.

For the coffee shop example above, you would enter `binompdf(5, 0.3, 2)`, which returns 0.3087.

### Excel
1. Click on an empty cell where you want the result to appear.
2. Type the following formula, then press Enter:
  - `=BINOM.DIST(k, n, p, FALSE)`
  - $k$ = number of successes, $n$ = number of trials, $p$ = probability of success
  - The **FALSE** tells Excel you want the probability of *exactly* $k$ successes (not cumulative).
3. For the coffee shop example, you would type `=BINOM.DIST(2, 5, 0.3, FALSE)`, which returns 0.3087.

### Desmos
Desmos doesn't have a single built-in binomial command, but it can calculate the formula directly using `nCr` (or `nCk`, depending on your Desmos update) for the combination.

1. In a blank expression line, type: `nCr(n,k)*p^k*(1-p)^(n-k)`, substituting your actual values of $n$, $p$, and $k$.
2. For the coffee shop example, type `nCr(5,2)*0.3^2*(1-0.3)^(5-2)`. Desmos will display the result, 0.3087, immediately.
