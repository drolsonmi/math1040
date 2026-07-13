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

# Lesson 10.4 Two Events: "AND" Probabilities
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1.3 Probabilities when events are not disjoint(pages 92-94)
* 3.2.4 General multiplication rule (pages 103-104)
* 3.1.5 Independence (pages 96-98)
* 3.2.6 Checking for independent and mutually exclusive events (pages 106-108)

## Lesson
Rearranging the conditional probability equation, we find a way to calculate "AND" probabilities:

$$P(B|A) = \frac{P(A~AND~B)}{P(A)} \qquad\to\qquad P(A~AND~B)=P(A)\cdot P(B|A)$$

In words: to find the probability of two events happening together, multiply the probability of the first event by the conditional probability of the second event, *given* that the first one happened.
 
### Why We Need the Conditional Piece
 
It's tempting to just multiply $P(A) \cdot P(B)$ directly, but that's only correct when $A$ and $B$ are **independent** (we'll define this precisely in 10.5). Whenever one event affects the probability of the other — like drawing cards or marbles **without replacement** — we have to use the conditional probability $P(B|A)$, not the plain probability $P(B)$.
 
### Example: Marbles Without Replacement
 
Recall from 10.3: a bag has 5 red marbles and 3 blue marbles (8 total), and we draw two marbles without replacement. What is $P(\text{first is red AND second is blue})$?
 
We already found $P(\text{first red}) = \frac{5}{8}$ and $P(\text{second blue} \mid \text{first red}) = \frac{3}{7}$. Multiplying these together:
 
$$P(\text{first red and second blue}) = P(\text{first red}) \cdot P(\text{second blue} \mid \text{first red}) = \frac{5}{8}\cdot\frac{3}{7} = \frac{15}{56} \approx 0.268$$
 
### Example: Using a Two-Way Table to Check the Rule
 
We can also use the multiplication rule to *confirm* a value we could otherwise read straight from a table. Recall our survey table from 10.1:
 
| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |
 
We already know $P(\text{car}) = 0.5$ and, from 10.3, $P(\text{job} \mid \text{car}) = 0.6$. Using the multiplication rule:
 
$$P(\text{car and job}) = P(\text{car}) \cdot P(\text{job} \mid \text{car}) = (0.5)(0.6) = 0.3$$
 
This matches exactly what we'd get by reading the table directly: $\frac{60}{200} = 0.3$. This is a useful way to double-check your conditional probability calculations.

<iframe width="560" height="315" src="https://www.youtube.com/embed/dfyN2HU3ZSs?si=P2HS4iB4tDZWOEd5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. Using the survey table below, we know $P(\text{no car}) = 0.5$ and $P(\text{no job} \mid \text{no car}) = 0.5$. Use the multiplication rule to find $P(\text{no car and no job})$, then check your answer against the table.
    | | Has a Job | No Job | Total |
    | --- | --- | --- | --- |
    | **Owns a Car** | 60 | 40 | 100 |
    | **No Car** | 50 | 50 | 100 |
    | **Total** | 110 | 90 | 200 |
 
  - [After solving on your own, see solution here](./Solutions/10_4_Solution1.html)
2. A bag contains 5 red marbles and 3 blue marbles. Two marbles are drawn **without replacement**. Find $P(\text{first is blue AND second is red})$.
  - [After solving on your own, see solution here](./Solutions/10_4_Solution2.html)
3. Two cards are drawn **without replacement** from a standard 52-card deck. Find $P(\text{both cards are Kings})$.
  - [After solving on your own, see solution here](./Solutions/10_4_Solution3.html)
4. A fair coin is flipped, and a fair six-sided die is rolled. These two events don't affect each other at all. Find $P(\text{coin shows heads AND die shows a 6})$.
  - [After solving on your own, see solution here](./Solutions/10_4_Solution4.html)
 
