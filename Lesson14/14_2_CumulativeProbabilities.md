<head>
<title>Lesson 14.2 Cumulative Probabilities from any Discrete Probability Distribution</title>
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

# Lesson 14.2 Cumulative Probabilities from any Discrete Probability Distribution
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.4.1 Bernoulli random variables and the binomial distribution

## Lesson
So far, whenever we've had a probability distribution table, we've only asked about one value of $x$ at a time. But very often, the real question is about a whole __range__ of values: "at least," "at most," "more than," "fewer than," or "between." A probability that covers a range of outcomes like this is called a __cumulative probability__.

Because the different values of a discrete random variable are mutually exclusive (lesson 14.1), a cumulative probability is nothing more than adding up the individual probabilities of every value of $x$ that fits the range. This idea works for **any** discrete probability distribution, not just the binomial distribution we'll return to in the next section.

### Translating Words into Math

| Phrase | Meaning | How to calculate |
| --- | --- | --- |
| "at least $x$" | $x$ or more | $P(x) + P(x+1) + \dots + P(n)$ |
| "at most $x$" | $x$ or fewer | $P(0) + P(1) + \dots + P(x)$ |
| "more than $x$" | strictly greater than $x$ | $P(x+1) + P(x+2) + \dots + P(n)$ |
| "fewer than $x$" / "less than $x$" | strictly less than $x$ | $P(0) + P(1) + \dots + P(x-1)$ |
| "between $a$ and $b$" (inclusive) | $a$ through $b$ | $P(a) + P(a+1) + \dots + P(b)$ |

A very useful shortcut comes from the Complement Rule (lesson 9): since all the probabilities in a distribution must add to 1, "at least $x$" is always the complement of "fewer than $x$" (at most $x-1$):

$$P(x \geq x_0) = 1 - P(x \leq x_0 - 1)\tag{Complement Shortcut}$$

This is often the fastest way to calculate an "at least" probability, especially when $x_0$ is small and there would otherwise be many terms to add.

### Worked Example

A discrete random variable $x$ has the distribution below.

| $x$ | 0 | 1 | 2 | 3 | 4 |
| --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.08 | 0.22 | 0.35 | 0.25 | 0.10 |

Find $P(x \leq 2)$ ("at most 2"):

$$P(x\leq 2) = P(0)+P(1)+P(2) = 0.08+0.22+0.35 = 0.65$$

Find $P(x \geq 3)$ ("at least 3"), two ways:

$$P(x\geq 3) = P(3)+P(4) = 0.25+0.10 = 0.35$$

$$P(x\geq 3) = 1-P(x\leq 2) = 1-0.65 = 0.35 \checkmark$$

Both methods agree, as they should.

<iframe width="560" height="315" src="https://www.youtube.com/embed/xxKW1a1kUxU?si=SefEEZOpV3F0nB9x" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
A small college's IT help desk keeps track of how many support tickets, $x$, come in per hour. The probability distribution is given below.

| $x$ | 0 | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.05 | 0.15 | 0.30 | 0.25 | 0.15 | 0.10 |

1. Find the probability that **at most 2** tickets come in during a given hour.
  - [After solving on your own, see solution here](./Solutions/14_2_Solution1.html)
2. Find the probability that **more than 3** tickets come in during a given hour.
  - [After solving on your own, see solution here](./Solutions/14_2_Solution2.html)
3. Find the probability that **between 1 and 3** tickets (inclusive) come in during a given hour.
  - [After solving on your own, see solution here](./Solutions/14_2_Solution3.html)
4. Find the probability that **at least 1** ticket comes in during a given hour, using the Complement Shortcut.
  - [After solving on your own, see solution here](./Solutions/14_2_Solution4.html)
