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

# Lesson 16.1 Practice Calculating Probabilities
On this page, we will be practicing using Normal Distributions. We will practice with the following question:
> The average number of calories in a 1.5-ounce chocolate bar is $\mu=210$. Suppose that the distribution of calories is approximately normal with $\sigma=10$. 

<!--Probabilities Left of Value-->
1. Find the probability that a randomly selected chocolate bar will have less than 200 calories.
$$z = \frac{200 - 210}{10} = \frac{-10}{10} = -1$$
$$P(z < -1) = 0.1587 = 15.87\%$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ha1ClYEy_LM?si=hKi7FjGa8kNZLsr5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<!--Probabilities Right of Value-->
2. Find the probability that a randomly selected chocolate bar will have more than 225 calories.
$$z = \frac{225 - 210}{10} = \frac{15}{10} = 1.5$$
$$P(z > 1.5) = 1 - P(z < 1.5) = 1 - 0.9332 = 0.0668 = 6.68\%$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/dc8rolSPfgA?si=ysbk01E-e8VvJeyd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<!--Probabilities Between Two Values-->
3. Find the probability that a randomly selected chocolate bar will have between 200 and 220 calories.
$$z_a = \frac{200 - 210}{10} = \frac{-10}{10} = -1$$
$$z_b = \frac{220 - 210}{10} = \frac{10}{10} = 1$$
$$P(z < 1) = 0.8413 \qquad P(z < -1) = 0.1587$$
$$P(-1 < z < 1) = P(z < 1) - P(z < -1) = 0.8413 - 0.1587 = 0.6826 = 68.26\%$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/sUu8M82s-xM?si=d_kwUbVOSpdzTSgV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

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