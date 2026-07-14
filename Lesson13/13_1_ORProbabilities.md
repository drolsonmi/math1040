<head>
<title>Lesson 13.1 Review of OR Probabilities</title>
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

# Lesson 13.1 Review of "OR" Probabilities
## Reading
This is a review of material from [Lesson 10](../Lesson10/index.md). If you would like to revisit the original reading, it comes from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1 Defining probability (pages 81-94)

## Lesson
Back in lesson 10, we learned how to find the probability that *at least one* of two events happens — this is the "OR" probability, also called the __addition rule__.

$$P(A \text{ or } B) = P(A) + P(B) - P(A \text{ and } B)\tag{General Addition Rule}$$

We also learned that when two events are __mutually exclusive__ (they cannot both happen at the same time), the overlap $P(A \text{ and } B)$ is 0, and the rule simplifies:

$$P(A \text{ or } B) = P(A) + P(B)\tag{Addition Rule for Mutually Exclusive Events}$$

This simplified version extends to any number of mutually exclusive events. If $A$, $B$, and $C$ are all mutually exclusive of one another, then:

$$P(A \text{ or } B \text{ or } C) = P(A) + P(B) + P(C)$$

### Why We're Reviewing This Now

Over the next two lessons, we're going to build __binomial probabilities__ — the probability of getting a specific number of "successes" out of a set number of trials. A single value, like "exactly 3 successes," is one outcome. But later in lesson 13.3, we will need to answer questions like:

> What is the probability that, out of 20 people, 3, 4, *or* 5 of them are successes?

Getting exactly 3 successes, exactly 4 successes, and exactly 5 successes are three separate, mutually exclusive outcomes — you can't have exactly 3 successes *and* exactly 4 successes in the same sample. That means once we know the individual probabilities, we can find the probability of "3, 4, or 5" simply by **adding them together**, exactly like we did in lesson 10.

$$P(3 \text{ or } 4 \text{ or } 5) = P(3) + P(4) + P(5)$$

Keep this idea in the back of your mind as we move into binomial probabilities — we'll come back to it in lesson 13.3.

## Practice
1. A survey of registered voters finds that 40% support Proposal A and 25% support Proposal B. No voter supports both proposals (they are mutually exclusive positions). What is the probability that a randomly selected voter supports Proposal A or Proposal B?
  - [After solving on your own, see solution here](./Solutions/13_1_Solution1.html)
2. A jar of marbles contains only red, blue, and green marbles. The probability of drawing a red marble is 0.3, and the probability of drawing a blue marble is 0.45. What is the probability of drawing a red or a blue marble? What is the probability of drawing a green marble?
  - [After solving on your own, see solution here](./Solutions/13_1_Solution2.html)
3. A die is rolled once. Let event $A$ = "rolling an even number" and event $B$ = "rolling a number greater than 4." Are $A$ and $B$ mutually exclusive? Find $P(A \text{ or } B)$.
  - [After solving on your own, see solution here](./Solutions/13_1_Solution3.html)
