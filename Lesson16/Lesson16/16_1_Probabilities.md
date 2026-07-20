<head>
<title>Lesson 16.1 Practice Calculating Probabilities</title>
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

# Lesson 16.1 Practice Calculating Probabilities

On this page, we will be practicing using Normal Distributions. We will practice with the following question:
> The average number of calories in a 1.5-ounce chocolate bar is $\mu=210$. Suppose that the distribution of calories is approximately normal with $\sigma=10$.

1. Find the probability that a randomly selected chocolate bar will have less than 200 calories.

This is a "less than" question, so we just need the z-score and the area to its left.

$$z = \frac{200 - 210}{10} = \frac{-10}{10} = -1$$

$$P(z < -1) = 0.1587 = 15.87\%$$

[https://www.youtube.com/embed/Ha1ClYEy_LM?si=hKi7FjGa8kNZLsr5](https://www.youtube.com/embed/Ha1ClYEy_LM?si=hKi7FjGa8kNZLsr5)

2. Find the probability that a randomly selected chocolate bar will have more than 225 calories.

This is a "more than" question. The Z-table only gives area to the left, so we find the area to the left and subtract from 1.

$$z = \frac{225 - 210}{10} = \frac{15}{10} = 1.5$$

$$P(z > 1.5) = 1 - P(z < 1.5) = 1 - 0.9332 = 0.0668 = 6.68\%$$

[https://www.youtube.com/embed/dc8rolSPfgA?si=ysbk01E-e8VvJeyd](https://www.youtube.com/embed/dc8rolSPfgA?si=ysbk01E-e8VvJeyd)

3. Find the probability that a randomly selected chocolate bar will have between 200 and 220 calories.

This is a "between" question, so we find both z-scores and subtract the smaller area from the larger one.

$$z_a = \frac{200 - 210}{10} = \frac{-10}{10} = -1$$

$$z_b = \frac{220 - 210}{10} = \frac{10}{10} = 1$$

$$P(z < 1) = 0.8413 \qquad P(z < -1) = 0.1587$$

$$P(-1 < z < 1) = P(z < 1) - P(z < -1) = 0.8413 - 0.1587 = 0.6826 = 68.26\%$$

[https://www.youtube.com/embed/sUu8M82s-xM?si=d_kwUbVOSpdzTSgV](https://www.youtube.com/embed/sUu8M82s-xM?si=d_kwUbVOSpdzTSgV)

## Technology

### TI-83/84

- Press `2nd`, then `VARS` to open the `DISTR` menu
- Choose `2:normalcdf(`
- Enter the lower bound, upper bound, mean, and standard deviation, separated by commas: `normalcdf(lower, upper, mean, st.dev.)`
  * For a "less than" probability, use a very small lower bound, like `-1E99`
  * For a "greater than" probability, use a very large upper bound, like `1E99`
- Press `ENTER`

### Excel

- Use `=NORM.DIST(x, mean, standard_dev, TRUE)` to find the area to the LEFT of $x$
- For "greater than," subtract from 1: `=1-NORM.DIST(x, mean, standard_dev, TRUE)`
- For "between," subtract the smaller cumulative area from the larger one: `=NORM.DIST(upper, mean, standard_dev, TRUE)-NORM.DIST(lower, mean, standard_dev, TRUE)`

### Desmos

- Type an expression using `normaldist(mean, standard_dev).cdf([lower, upper])`
  * For example, `normaldist(210,10).cdf([-1000,200])` finds the probability of getting less than 200 calories
- Desmos will return the area (probability) directly

## Practice

1. The length of a human pregnancy is approximately normally distributed with $\mu = 268$ days and $\sigma = 15$ days. Find the probability that a randomly selected pregnancy lasts **less than 250 days**.
  - [After solving on your own, see solution here](./Solutions/16_1_Solution1.html)
2. SAT Math scores are approximately normally distributed with $\mu = 520$ and $\sigma = 100$. Find the probability that a randomly selected student scores **more than 650**.
  - [After solving on your own, see solution here](./Solutions/16_1_Solution2.html)
3. The battery life of a certain phone model is approximately normally distributed with $\mu = 11$ hours and $\sigma = 1.2$ hours. Find the probability that a randomly selected phone's battery lasts **between 9 and 12 hours**.
  - [After solving on your own, see solution here](./Solutions/16_1_Solution3.html)
4. Daily household water usage in a city is approximately normally distributed with $\mu = 300$ gallons and $\sigma = 40$ gallons. Find the probability that a randomly selected household uses **more than 380 gallons** in a day.
  - [After solving on your own, see solution here](./Solutions/16_1_Solution4.html)
