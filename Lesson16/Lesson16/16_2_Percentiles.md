<head>
<title>Lesson 16.2 Practice Calculating Percentiles/Quartiles</title>
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

On the last page, we looked at using Normal Distributions to calculate probabilities. On this page, we will continue this study by looking at percentiles, or calculating values which border on areas.

We'll continue with the problem we worked on last time:
> The average number of calories in a 1.5-ounce chocolate bar is $\mu=210$. Suppose that the distribution of calories is approximately normal with $\sigma=10$.

1. How many calories are in the 75th percentile?

The 75th percentile is the value with 75% of the data below it, so we first find the z-score with 0.75 area to its left, then convert that z-score into a value.

- That is, what value is above the lower 75% of the graph?

$$P(z<a) = 0.75 \qquad a = ?$$

$$\text{Using a Z-table, }a = 0.675$$

$$0.675 = \frac{x - 210}{10} \qquad\to\qquad x = 210 + 10(0.675) = 216.75$$

[https://www.youtube.com/embed/cpvJ0m_-xAA?si=QFbHkKcBda7sfY9Y](https://www.youtube.com/embed/cpvJ0m_-xAA?si=QFbHkKcBda7sfY9Y)

2. How many calories are in the lowest (1st) quartile?

Quartiles are just specific percentiles: $Q_1$ is the 25th percentile, $Q_2$ (the median) is the 50th percentile, and $Q_3$ is the 75th percentile.

  - The 1st quartile is the lowest 25%
  - Thus, the 1st quartile is equal to the 25th percentile
  - So, what value is above the lower 25% of the graph?

$$P(z<a) = 0.25 \qquad a = ?$$

$$\text{Using a Z-table, }a = -0.675$$

$$-0.675 = \frac{x - 210}{10} \qquad\to\qquad x = 210 + 10(-0.675) = 203.25$$

[https://www.youtube.com/embed/kQ9cBy4tcQE?si=B1JOFCvnhkJGTZ0m](https://www.youtube.com/embed/kQ9cBy4tcQE?si=B1JOFCvnhkJGTZ0m)

