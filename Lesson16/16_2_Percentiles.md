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

# Lesson 16.2 Practice Calculating Percentiles/Quartiles
On the last page, we looked at using Normal Distributions to calculation probabilities. On this page, we will continue this study by looking at percentiles, or calculating values which border on areas.

We'll continue with the problem we worked on last time:
> The average number of calories in a 1.5-ounce chocolate bar is $\mu=210$. Suppose that the distribution of calories is approximately normal with $\sigma=10$. 

<!--Percentiles-->
1. How many calories are in the 75th percentile?
    * That is, what value is above the lower 75% of the graph?
    $$P(z<a) = 0.75 \qquad a = ?$$
    $$\text{Using a Z-table, }a = 0.675$$
    $$0.675 = \frac{x - 210}{10} \qquad\to\qquad x = 210 + 10*0.675 = 216.75$$
<iframe width="560" height="315" src="https://www.youtube.com/embed/cpvJ0m_-xAA?si=QFbHkKcBda7sfY9Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


<!--Quartiles-->
2. How many calories are in the lowest (1st) quartile?
    * The 1st quartile is the lowest 25%
    * Thus, the 1st quartile is equal to the 25th percentile
    * So, what value is above the lower 25% of the graph?
    $$P(z<a) = 0.75 \qquad a = ?$$
    $$\text{Using a Z-table, }a = -0.675$$
    $$-0.675 = \frac{x - 210}{10} \qquad\to\qquad x = 210 + 10*(-0.675) = 203.25$$
<iframe width="560" height="315" src="https://www.youtube.com/embed/kQ9cBy4tcQE?si=B1JOFCvnhkJGTZ0m" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<!--
## Practice
1. ?
    * After solving on your own, [check the solution](Solutions/20_1_Solution1.md).
2. ?
    * After solving on your own, [check the solution](Solutions/20_1_Solution2.md).
3. ?
    * After solving on your own, [check the solution](Solutions/20_1_Solution3.md).
-->

<!--
## Technology

### TI-83/84

### Excel

### Desmos
-->