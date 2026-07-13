<head>
<title>Lesson 9 Probability</title>
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

# Lesson 9 Probability
In segment 2, we were able to do calculations on quantitative data to get an idea of the behavior of those variables. The disadvantage to categorical variables is that it is not easy to do calculations. For example, what is the average of this dataset of grade level {Freshman, Sophomore, Sophomore, Junior, Senior, Senior} ? At first glance, this isn't possible. However, we do have one tool that will help us to do some calculations: probabilities.

In this lesson, we will learn about relative frequency, probability, and the relationship between the two.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_SZHkZijpiw?si=IRBXjclpQSiWeKbj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

A few important definitions for this lesson:
* __Event__: An action that results in one of multiple possible outcomes
    * Example: Rolling a die
* __Outcome__: A possible result from an event
    * Example: Rolling a (5) on a die
* __Sample Space__: The list of possible outcomes
    * Example: Rolling a die, the sample space is any possible number: {1, 2, 3, 4, 5, 6}
* __Relative Frequency__: The percentage of time that an outcome occurs
    * Example: You roll a die 60 times
        * Of those rolls, 13 of them are a (5)
        * The relative frequency is 13 out of 60, or $$\tfrac{13}{60} = 0.2167 = 21.67\%$$
    * Note: the term "percent" literally means "per 100". So, $$0.37 = \tfrac{37}{100}$$ would be read as 37 per 100, or 37%.
* __Probability__: The fraction of possible outcomes that would constitute a success
    * Example: You want to roll a number larger than 2.
        * There are 6 possible outcomes: {1, 2, 3, 4, 5, 6} (This is your Sample Space)
        * There are 4 possible successful outcomes that would be a number larger than 2: {3, 4, 5, 6}
        * The probability would be $$\frac{size\{3,4,5,6\}}{size\{1,2,3,4,5,6\}} = \frac{4}{6}=\frac{2}{3}=0.667 = 66.7\%$$

## Outcomes
By the end of this lesson, you should be able to accomplish the following:
 
- Identify the sample space, outcomes, and events associated with a random process
- Calculate the theoretical probability of an event, and explain why probabilities must always fall between 0 and 1
- Calculate the relative frequency of an event from observed data, and explain how it differs from theoretical probability
- Calculate the complement of an event and use the complement rule, $P(A') = 1 - P(A)$, to simplify probability calculations

## Topics in this lecture
* [9.1 Probability](./9_1_Probability.md)
* [9.2 Relative Frequency (Proportions)](./9_2_RelativeFrequency.md)
* [9.3 Complements](./9_3_Complements.md)