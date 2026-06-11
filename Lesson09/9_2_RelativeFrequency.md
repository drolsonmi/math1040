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

# Lesson 9.2 Relative Frequency (Proportions)
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.1.1 Probability (pages 88-90)

## Lesson
A __Probability__ is the ratio of the number of successful outcomes to the number possible outcomes. However, if you do an experiment in real life, the randomness causes numbers to not always follow probabilities. For example, if I roll a die 100 times and count the 5's, I could get 20 out of the 100 rolls as 5 even though the probability of rolling a 5 says I should have 16.67 rolls of my 100 be 5's.

In that example, we saw what is called the __Relative Frequency__, or the fraction of events that match our successful outcome. To calculate the relative frequency, take the number of successes in your event and divide it by the total number of events.

> Example 1: You have a bucket of 6-sided dice. You just dump them out then count the occurrences of each number. This table displays the counts:
> 
> | Roll  | 1     | 2     | 3     | 4     | 5     | 6     |
> | :---- | :---: | :---: | :---: | :---: | :---: | :---: |
> | Count | 83    | 48    | 27    | 12    | 76    | 33    |
>
> Adding these up, there is a total of 279 rolls. So, the relative frequencies are:
> 
> | Roll  | Count | Relative Frequency     |
> | :---: | :---: | :--------------------- |
> | 1     | 83    | 83/279 = 0.297 = 29.7% |
> | 2     | 48    | 48/279 = 0.172 = 17.2% |
> | 3     | 27    | 27/279 = 0.097 = 9.7%  |
> | 4     | 12    | 12/279 = 0.043 = 4.3%  |
> | 5     | 76    | 76/279 = 0.272 = 27.2% |
> | 6     | 33    | 33/279 = 0.118 = 11.8% |

This table is what we call a Probability Distribution. We will see them more in Lesson 12. But for now, note the following 2 rules of probability distributions:
* All relative frequencies (or probabilities) must be between 0 and 1 (that is, 0% and 100%) - no negatives and nothing larger than 1.
* All relative frequencies (or probabilities) must add up to 1 (100%).
 
> Example 2: There are 15 students in a class. Below is a table of their grade levels:
> 
> | Grade | Freshman | Sophomore | Junior | Senior |
> | :---- | :------: | :-------: | :----: | :----: |
> | Count | 4        | 8         | 2      | 1      |
>
> The relative frequencies are just the number in each class divided by the total of 15:
> 
> | Grade     | Count | Relative Frequency   |
> | :-------- | :---: | :------------------- |
> | Freshman  | 4     | 4/15 = 0.267 = 26.7% |
> | Sophomore | 8     | 8/15 = 0.533 = 53.3% |
> | Junior    | 2     | 2/15 = 0.133 = 13.3% |
> | Senior    | 1     | 1/15 = 0.067 = 6.7%  |

<iframe width="560" height="315" src="https://www.youtube.com/embed/dbgpIuX7Rdg?si=7XPgOb-kh-OlPJJq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
### Practice Question 9.2.1
1. A survey was conducted to find out people's preferred type of pet. The results are as follows:

| Pet Type | People who prefer pet |
| :------- | :-------------------: |
| Dogs     | 40 people             |
| Cats     | 25 people             |
| Birds    | 10 people             |
| Fish     | 15 people             |
| Reptiles | 10 people             |

After solving on your own, [check the solution](Solutions/9_2_Solution1.md).

2. You have a large bag of colored marbles. You randomly grab a handful of marbles and count the colors. Calculate the relative frequency of each color:

| Color | Red   | Blue  | Green | Yellow | Black | White |
| :---- | :---: | :---: | :---: | :----: | :---: | :---: |
| Count | 22    | 13    | 10    | 9      | 7     | 18    |

After solving on your own, [check the solution](Solutions/9_2_Solution2.md).

3. A teacher recorded the number of books read by students in five different genres over the course of a semester. The data is shown below:

| Genre | Fiction | Non-Fiction | Mystery | Science Fiction | Biography |
| :---- | :-----: | :---------: | :-----: | :-------------: | :-------: |
| Count | 24      | 18          | 12      | 6               | 10        |

After solving on your own, [check the solution](Solutions/9_2_Solution3.md).

<!--
## Technology

### TI-83/84

### Excel

### Desmos
-->