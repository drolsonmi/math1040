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

# Lesson 10.5 Independent Events
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1.3 Probabilities when events are not disjoint(pages 92-94)
* 3.1.5 Independence (pages 96-98 of the [Introductory Statistics Textbook](OpenIntroTextbook.pdf))
* 3.2.6 Checking for independent and mutually exclusive events (pages 106-108)

## Lesson
Conditional probabilities happen when the probability of one event depends on the occurrence of another event.
 
However, there are some events that do not depend on another event. If this is the case, then an event's conditional probability is the same as the probability of the event itself.
 
$$P(B|A) = P(B)$$
 
In other words, event B doesn't change whether event A happens or not. When this is true, we say $A$ and $B$ are **independent events**.
 
### Testing for Independence
 
To check whether two events are independent, compare the conditional probability $P(B|A)$ to the plain probability $P(B)$:
 
- If $P(B|A) = P(B)$, the events are **independent**.
- If $P(B|A) \ne P(B)$, the events are **dependent**.
Recall our survey table of 200 college students:
 
| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |
 
In 10.3, we calculated $P(\text{job}) = 0.55$ and $P(\text{job} \mid \text{car}) = 0.6$. Since these two values are **not equal**, owning a car and having a job are **dependent** events — knowing a student owns a car actually shifts the probability that they have a job.
 
Compare that to flipping a coin and rolling a die, from 10.4: we found $P(6) = \frac{1}{6}$ and $P(6 \mid \text{heads}) = \frac{1}{6}$. Since these values **are equal**, the coin flip and die roll are **independent** — knowing the coin landed heads tells us nothing about the die.
 
### A Simplified Multiplication Rule
 
When two events are independent, the general multiplication rule from 10.4 simplifies, since $P(B|A)$ is just $P(B)$:
 
$$P(A~AND~B) = P(A)\cdot P(B|A) \qquad\Longrightarrow\qquad P(A~AND~B) = P(A)\cdot P(B) \quad \text{(independent events only)}$$
 
This is why we were able to simply multiply $P(\text{heads}) \cdot P(6)$ directly in 10.4 — no conditional probability was needed, because the two events were independent.
 
### With Replacement vs. Without Replacement
 
A helpful way to build intuition: drawing cards or marbles **with replacement** (putting an item back before the next draw) creates **independent** events, since the sample space resets each time. Drawing **without replacement** creates **dependent** events, since removing an item changes what's left for the next draw. This is exactly why our marble and card examples from 10.3 and 10.4 needed conditional probabilities — we never put anything back.

<iframe width="560" height="315" src="https://www.youtube.com/embed/NNjgaYUA0k8?si=1UM3QMqby74sJNoo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. Using the survey table below, determine whether "owns a car" and "has a job" are independent events. Show your work by comparing $P(\text{car})$ to $P(\text{car} \mid \text{job})$.
    | | Has a Job | No Job | Total |
    | --- | --- | --- | --- |
    | **Owns a Car** | 60 | 40 | 100 |
    | **No Car** | 50 | 50 | 100 |
    | **Total** | 110 | 90 | 200 |
 
  - [After solving on your own, see solution here](./Solutions/10_5_Solution1.html)
2. A fair coin is flipped, and a fair six-sided die is rolled. Show that these two events are independent by comparing $P(\text{6})$ to $P(\text{6} \mid \text{heads})$, then use the simplified multiplication rule to find $P(\text{tails AND rolling a 3})$.
  - [After solving on your own, see solution here](./Solutions/10_5_Solution2.html)
3. Two cards are drawn from a standard 52-card deck. Compare the following two scenarios, and explain why one produces independent events while the other does not:
  - **Scenario A**: A card is drawn, put back in the deck (with replacement), and then a second card is drawn. Find $P(\text{second is a King} \mid \text{first is a King})$.
  - **Scenario B**: A card is drawn and **not** put back (without replacement), and then a second card is drawn. Find $P(\text{second is a King} \mid \text{first is a King})$.
  - [After solving on your own, see solution here](./Solutions/10_5_Solution3.html)