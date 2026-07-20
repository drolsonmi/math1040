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

## Technology

These problems work in the opposite direction from Lesson 16.1: instead of starting with a value and finding an area, we start with an area (the percentile, as a decimal) and find the value.

### TI-83/84

- Press `2nd`, then `VARS` to open the `DISTR` menu
- Choose `3:invNorm(`
- Enter the area to the LEFT, the mean, and the standard deviation, separated by commas: `invNorm(area, mean, st.dev.)`
- Press `ENTER`

### Excel

- Use `=NORM.INV(probability, mean, standard_dev)`, where `probability` is the area to the LEFT
  * For example, `=NORM.INV(0.9,520,100)` returns the value at the 90th percentile of a distribution with mean 520 and standard deviation 100

### Desmos

- Type an expression using `normaldist(mean, standard_dev).inversecdf(probability)`
  * For example, `normaldist(520,100).inversecdf(0.9)` returns the value at the 90th percentile

## Practice

1. The length of a human pregnancy is approximately normally distributed with $\mu = 268$ days and $\sigma = 15$ days. Doctors flag a pregnancy as unusually early if it falls in the lowest 10% of lengths. Find the length that marks the **10th percentile**.
  - [After solving on your own, see solution here](./Solutions/16_2_Solution1.html)
2. SAT Math scores are approximately normally distributed with $\mu = 520$ and $\sigma = 100$. A scholarship committee wants to award scholarships to the top 10% of scorers. Find the minimum score needed, i.e. the **90th percentile**.
  - [After solving on your own, see solution here](./Solutions/16_2_Solution2.html)
3. The battery life of a certain phone model is approximately normally distributed with $\mu = 11$ hours and $\sigma = 1.2$ hours. Find the **3rd quartile ($Q_3$)** of battery life.
  - [After solving on your own, see solution here](./Solutions/16_2_Solution3.html)
4. Daily household water usage in a city is approximately normally distributed with $\mu = 300$ gallons and $\sigma = 40$ gallons. Find the **1st quartile ($Q_1$)** of daily water usage.
  - [After solving on your own, see solution here](./Solutions/16_2_Solution4.html)
