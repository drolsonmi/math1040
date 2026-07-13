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

# Lesson 10.1 Two Events: "OR" Probabilities
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1.2 Disjoint or mutually exclusive outcomes (pages 90-92)

## Lesson
When we ask about the probability of one event OR another event, we count both groups as successful outcomes. So, we can add their individual probabilities together.

$$P(A~OR~B) = P(A)+P(B)$$

However, there is a chance that some outcomes can occur in both events. When this happens, any events that happen in both categories are counted twice. So, we subtract one out so it is only counted once.

$$P(A~OR~B) = P(A)+P(B)-P(A~AND~B)$$

This is the full equation for "OR" probabilities.

<iframe width="560" height="315" src="https://www.youtube.com/embed/FcCjfTRqCIk?si=3Ev9WyxYx-8tWb5R" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Why Do We Subtract the Overlap?
 
Picture drawing one card from a standard deck and asking for $P(\text{King OR Heart})$. There are 4 Kings and 13 Hearts, but if we just add $4 + 13 = 17$, we've actually counted the King of Hearts **twice** — once as a King, and once as a Heart. Since it's only one card, we need to subtract that overlap out once:
 
$$P(\text{King or Heart}) = P(\text{King}) + P(\text{Heart}) - P(\text{King and Heart}) = \frac{4}{52} + \frac{13}{52} - \frac{1}{52} = \frac{16}{52} \approx 0.308$$
 
A **two-way table** (sometimes called a contingency table) is a useful way to organize compound probability problems, since it shows every combination of two categorical variables at once. For example, suppose we surveyed 200 college students about whether they own a car and whether they have a part-time job:
 
| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |
 
To find $P(\text{owns a car OR has a job})$, we can read the needed values directly from the table:
 
$$P(\text{car}) = \frac{100}{200} = 0.5, \qquad P(\text{job}) = \frac{110}{200} = 0.55, \qquad P(\text{car and job}) = \frac{60}{200} = 0.3$$
 
$$P(\text{car or job}) = 0.5 + 0.55 - 0.3 = 0.75$$
 
We'll use this same table again in the next few sections, since two-way tables make it easy to read off "AND," "OR," and conditional probabilities all from the same data.

## Practice
1. A single card is drawn from a standard 52-card deck. Find $P(\text{Jack OR Spade})$.
  - [After solving on your own, see solution here](./Solutions/10_1_Solution1.html)
2. Using the survey table from the lesson (200 college students, car ownership vs. part-time job):
    | | Has a Job | No Job | Total |
    | --- | --- | --- | --- |
    | **Owns a Car** | 60 | 40 | 100 |
    | **No Car** | 50 | 50 | 100 |
    | **Total** | 110 | 90 | 200 |
 
  - Find the probability that a randomly selected student **owns a car OR does not have a job**.
  - [After solving on your own, see solution here](./Solutions/10_1_Solution2.html)
3. A fair six-sided die is rolled once. Find $P(\text{rolling an even number OR rolling a number greater than 4})$.
  - [After solving on your own, see solution here](./Solutions/10_1_Solution3.html)
4. A factory inspects 300 items for two types of defects. 40 items have Defect A, 50 items have Defect B, and 15 items have both defects. Find the probability that a randomly selected item has **Defect A OR Defect B**.
  - [After solving on your own, see solution here](./Solutions/10_1_Solution4.html)
 