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

# Lesson 10.3 Conditional Probabilities
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.2.1 Conditional Probability (pages 98-100)
* 3.2.2 Defining conditional probability (pages 100-102)
* 3.2.4 General multiplication rule (pages 103-104)
* 3.2.7 Tree diagrams (pages 109-110)

## Lesson
When dealing with two events, there is a chance that one event could be affected by another event. For example, the clothes that you wear depend on how hot it is. In probability, we would ask, "What is the probability that we wear heavy coats __given that__ it is cold?" This is known as a __conditional probability__. We would write that as:

$$P(coat | cold)$$

The vertical bar symbol ( `|` ) means "given that". We can find a conditional probability as,

$$P(B|A) = \frac{P(A~AND~B)}{P(A)}$$

In words: a conditional probability **restricts our attention** to only the outcomes where $A$ already happened, and then asks what fraction of *those* outcomes also satisfy $B$.
 
### Using a Confusion Matrix (also called a Two-Way Table)
 
Conditional probabilities are especially easy to read from a __confusion matrix__, because $A$ tells us which row (or column) to restrict our attention to. Recall our survey of 200 college students:
 
| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |
 
Suppose we want $P(\text{has a job} \mid \text{owns a car})$ — given that a student owns a car, what's the probability they also have a job? Since we're told the student owns a car, we restrict our attention to just the "Owns a Car" row (100 students), and ask how many of those 100 also have a job (60):
 
$$P(\text{job} \mid \text{car}) = \frac{60}{100} = 0.6$$
 
We get the same answer using the formula directly:
 
$$P(\text{job} \mid \text{car}) = \frac{P(\text{car and job})}{P(\text{car})} = \frac{60/200}{100/200} = \frac{0.3}{0.5} = 0.6$$
 
Notice this is different from the *unconditional* probability of having a job, $P(\text{job}) = \frac{110}{200} = 0.55$. Knowing that a student owns a car actually **changed** the probability they have a job (from 55% up to 60%) — a sign that these two events might not be independent, which we'll explore further in 10.5.
 
### Conditional Probability with Sequential Events
 
Conditional probability also shows up whenever we draw items **without replacement**. For example, suppose a bag contains 5 red marbles and 3 blue marbles (8 total), and we draw two marbles without putting the first one back. What is $P(\text{second is blue} \mid \text{first is red})$?
 
Since the first marble drawn was red and *not* returned to the bag, only 7 marbles remain: 4 red and 3 blue.
 
$$P(\text{second blue} \mid \text{first red}) = \frac{3}{7} \approx 0.429$$
 
This idea — that removing an item changes the probabilities for the next draw — will be central to the "AND" probabilities we calculate in 10.4.

<iframe width="560" height="315" src="https://www.youtube.com/embed/jd_K5PfKHk0?si=pMWKGkl9PtR2Qsvt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
Use the survey table below (200 college students, car ownership vs. part-time job) for questions 1 and 2:
 
| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |
 
1. Find $P(\text{owns a car} \mid \text{no job})$.
  - [After solving on your own, see solution here](./Solutions/10_3_Solution1.html)
2. Find $P(\text{has a job} \mid \text{no car})$, and compare it to $P(\text{job})$.
  - [After solving on your own, see solution here](./Solutions/10_3_Solution2.html)
3. A single card is drawn from a standard 52-card deck. There are 12 face cards (Jacks, Queens, and Kings) in the deck. Find $P(\text{King} \mid \text{face card})$.
  - [After solving on your own, see solution here](./Solutions/10_3_Solution3.html)
4. A bag contains 5 red marbles and 3 blue marbles. Two marbles are drawn **without replacement**. Find $P(\text{second marble is blue} \mid \text{first marble is red})$.
  - [After solving on your own, see solution here](./Solutions/10_3_Solution4.html)
 