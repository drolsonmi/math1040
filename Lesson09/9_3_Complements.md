<head>
<title>Lesson 9.3 Complements</title>
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

# Lesson 9.3 Complements
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1.4 Complement of an event (page 95)

## Lesson
Sometimes the easiest way to find the probability of an event isn't to calculate that event directly — it's to calculate everything *else* and work backward. That's exactly what a complement lets us do.
 
### What Is a Complement?
 
The **complement** of an event $A$ is everything in the sample space that is **not** in $A$. We write the complement as $A'$ (read "A prime"), though you may also see it written as $A^c$ or $\bar{A}$.
 
For example, if we roll a die and let $A$ be the event "rolling a 6," then the complement $A'$ is the event "not rolling a 6" — in other words, rolling a 1, 2, 3, 4, or 5:
 
$$A = \{6\}, \qquad A' = \{1, 2, 3, 4, 5\}$$
 
Notice that together, an event and its complement always make up the **entire sample space**, with no overlap between them. Every outcome belongs to either $A$ or $A'$ — never both, and never neither.
 
### The Complement Rule
 
Since $A$ and $A'$ together account for 100% of the sample space, their probabilities must add up to 1:
 
$$P(A) + P(A') = 1$$
 
Rearranging this gives us the **Complement Rule**, which lets us find the probability of an event's complement — or the event itself — whenever we already know one of the two:
 
$$P(A') = 1 - P(A) \qquad \text{or equivalently} \qquad P(A) = 1 - P(A')$$
 
### A Quick Example
 
Suppose we roll a die and want $P(\text{not rolling a 6})$. We already know $P(\text{rolling a 6}) = \frac{1}{6}$, so:
 
$$P(\text{not rolling a 6}) = 1 - P(\text{rolling a 6}) = 1 - \frac{1}{6} = \frac{5}{6} \approx 0.833 = 83.3\%$$
 
### Why Complements Are Useful
 
For a simple event like rolling a single die, it's just as easy to count the complement directly as it is to use the rule. But complements become genuinely useful when the *event itself* is complicated to count, while its *complement* is simple. This comes up constantly with **"at least one"** problems. For example, finding the probability of flipping "at least one heads" in several coin flips would require adding up many different cases (exactly one heads, exactly two heads, and so on) — but the complement, "zero heads" (all tails), is just a single, simple case to calculate. We'll see this exact idea in the practice problems below.

<iframe width="560" height="315" src="https://www.youtube.com/embed/6dFyTcAZWyY?si=MHLHm2ZA9GNukklD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. A jar contains 4 red marbles, 6 blue marbles, and 10 green marbles. One marble is drawn at random. Use the complement rule to find the probability that the marble is **not red**.
    - [After solving on your own, see solution here](Solutions/9_3_Solution1.md)
2. A survey finds that the probability a randomly selected person prefers coffee over tea is $P(\text{coffee}) = 0.62$. Find the probability that a randomly selected person does **not** prefer coffee.
    - [After solving on your own, see solution here](Solutions/9_3_Solution2.md)
3. A fair six-sided die is rolled once. Let $A$ be the event "rolling less than 3." Find $P(A)$ and $P(A')$, and describe what outcomes make up the complement.
    - [After solving on your own, see solution here](Solutions/9_3_Solution3.md)
4. A fair coin is flipped twice. Find the probability of getting **at least one heads**, by first finding the probability of the complement (getting zero heads).
    - [After solving on your own, see solution here](Solutions/9_3_Solution4.md)
 