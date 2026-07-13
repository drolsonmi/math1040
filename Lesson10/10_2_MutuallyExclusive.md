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

# Lesson 10.2 Mutually Exclusive Events
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1.2 Disjoint or mutually exclusive outcomes (pages 90-92)

## Lesson
Two events are __Mutually Exclusive__ if they cannot occur at the same time. When this happens,

$$P(A~AND~B) = 0$$

When this occurs, the equation for the "OR" probability is,

$$P(A~OR~B) = P(A) + P(B)$$

### Recognizing Mutually Exclusive Events
 
The easiest way to check whether two events are mutually exclusive is to ask: **is there any outcome that belongs to both events at once?** If the answer is no, the events are mutually exclusive.
 
- **Mutually exclusive example**: Rolling a die and looking at "rolling a 1" vs. "rolling a 6." A single roll can't be both a 1 and a 6 at the same time, so these events are mutually exclusive.
- **Not mutually exclusive example**: Drawing a card and looking at "drawing a King" vs. "drawing a Heart." These events overlap, since the King of Hearts belongs to both — so they are **not** mutually exclusive. (This is exactly the example we worked through in 10.1.)
Categorical variables from a two-way table are usually **not** mutually exclusive with each other unless the table is specifically built that way — for example, in our car/job survey table from 10.1, "owns a car" and "has a job" are not mutually exclusive, since 60 students fall into both categories at once. On the other hand, the different *rows* of that same table (e.g., "owns a car" vs. "no car") **are** mutually exclusive with each other, since a student can't be in both the "owns a car" row and the "no car" row simultaneously.
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/d8FTanhfWB8?si=5qfDSVHxcFkvkrc5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Quick Example
 
What is $P(\text{rolling a 2 or rolling a 5})$ on a single die roll? Since a single roll can only show one number, these two events can never happen together, so they're mutually exclusive:
 
$$P(\text{2 or 5}) = P(2) + P(5) = \frac{1}{6} + \frac{1}{6} = \frac{2}{6} = \frac{1}{3} \approx 0.333$$


## Practice
1. A single card is drawn from a standard 52-card deck. Explain why "drawing a King" and "drawing a Queen" are mutually exclusive, then find $P(\text{King OR Queen})$.
  - [After solving on your own, see solution here](./Solutions/10_2_Solution1.html)
2. A fair six-sided die is rolled once. Find $P(\text{rolling a 1 OR rolling a 6})$.
  - [After solving on your own, see solution here](./Solutions/10_2_Solution2.html)
3. For each pair of events below, determine whether they are mutually exclusive. Explain your reasoning for each.
  - Drawing a card that is a Heart, or drawing a card that is a King.
  - Rolling an even number on a die, or rolling an odd number on a die.
  - A randomly selected student owns a car, or that same student has a part-time job.
  - [After solving on your own, see solution here](./Solutions/10_2_Solution3.html)
 