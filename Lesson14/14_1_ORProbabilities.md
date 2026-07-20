<head>
<title>Lesson 14.1 Review of OR Probabilities</title>
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

# Lesson 14.1 Review of OR Probabilities
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.2.1 Union of non-disjoint events

## Lesson
Back in [lesson 10](../Lesson10/index.html), we learned how to find the probability that __event A or event B__ occurs. Before we can talk about cumulative probabilities later in this lesson, it's worth taking a moment to review that idea, since a cumulative probability is really just a big "OR" statement in disguise — for example, "at least 3 successes" means "3 successes, OR 4 successes, OR 5 successes, ...".

### The General Addition Rule

For any two events $A$ and $B$:

$$P(A \text{ or } B) = P(A) + P(B) - P(A \text{ and } B)\tag{General Addition Rule}$$

We subtract $P(A \text{ and } B)$ because if we just add $P(A)$ and $P(B)$, we would count the outcomes where both $A$ and $B$ happen twice — once in each probability.

### Mutually Exclusive Events

Two events are __mutually exclusive__ (or disjoint) if they cannot both happen at the same time — that is, $P(A \text{ and } B) = 0$. When events are mutually exclusive, the general addition rule simplifies, since there's nothing to subtract:

$$P(A \text{ or } B) = P(A) + P(B)\tag{Addition Rule for Mutually Exclusive Events}$$

This simplified version is the one we will lean on heavily for the rest of this lesson. Notice that the outcomes of a discrete random variable (for example, $x=3$ successes and $x=4$ successes in a binomial experiment) are always mutually exclusive of each other — a single trial can't simultaneously produce exactly 3 successes *and* exactly 4 successes. This means that whenever we want the probability of "this value or that value" for a random variable, we can simply **add the individual probabilities together**.

### Worked Example

A six-sided die is rolled once. What is the probability of rolling a 2 **or** a 5?

Rolling a 2 and rolling a 5 cannot happen on the same roll, so these events are mutually exclusive.

$$P(2 \text{ or } 5) = P(2) + P(5) = \frac{1}{6}+\frac{1}{6} = \frac{2}{6} = \frac{1}{3}$$

What about the probability of rolling an even number **or** a number greater than 4? These events are *not* mutually exclusive, since 6 is both even and greater than 4.

$$P(\text{even}) = \frac{3}{6}, \qquad P(>4) = \frac{2}{6}, \qquad P(\text{even and} > 4) = P(6) = \frac{1}{6}$$

$$P(\text{even or} >4) = \frac{3}{6}+\frac{2}{6}-\frac{1}{6} = \frac{4}{6} = \frac{2}{3}$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/6xfyeixdz2E?si=uVvT4qU3ye_oz2h9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. A standard deck of 52 cards is shuffled, and one card is drawn. Find the probability that the card is a King **or** a Queen.
  - [After solving on your own, see solution here](./Solutions/14_1_Solution1.html)
2. A standard deck of 52 cards is shuffled, and one card is drawn. Find the probability that the card is a Heart **or** a Face card (Jack, Queen, or King).
  - [After solving on your own, see solution here](./Solutions/14_1_Solution2.html)
3. A discrete random variable $x$ has the probability distribution below.

| $x$ | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.10 | 0.25 | 0.30 | 0.20 | 0.15 |

  Find $P(x=2 \text{ or } x=4)$. Explain why you are able to simply add the two probabilities.
  - [After solving on your own, see solution here](./Solutions/14_1_Solution3.html)
