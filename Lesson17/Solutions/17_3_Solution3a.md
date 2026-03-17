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

#### Answer to Practice Problem 3
A coffee shop claims that the average temperature of its freshly brewed coffee is 160°F with a standard deviation of 5°F. A health inspector randomly samples 41 cups of coffee.

1. What is the probability that the temperature of a single cup is between 158°F and 162°F?
    * The probability is found by finding the area between the two values on a standardized normal distribution using a Z-Table or a calculator
        * On a Z-Table,
            * The z-score of 158$\degree$ is $z = \frac{158 - 160}{5} = \frac{-2}{5} = -0.40
            * The z-score of 162$\degree$ is $z = \frac{162 - 160}{5} = \frac{2}{5} = 0.40
            * Look up area left of z = -0.60
                * $P(z < -0.40) = 0.3446$
            * Look up area left of z = 0.60
                * $P(z < 0.40) = 0.6554$
            * Take the difference between the two
                * $P(-0.40 < z < 0.40) = P(z < 0.40) - P(z < -0.40) = 0.6554 - 0.3446 = 0.311$
        * On a TI-83/84, DISTR --> 2:normalcdf(
            * 2:normalcdf(158,162,160,5) if using the values from the problem
            * 2:normalcdf(0.3446,0.6554,0,1) if using the z-score (gives the same answer)
    * __Probability = 0.311 = 31.1%__

[Click here](../17_3_CentralLimitTheorem.md#practice) to return to the lecture notes.