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
<title>Solution for practice 17.4.3</title>
</head>

## 17.4 Example - Solution for Practice 3
The reaction time of frogs to a particular stimulus has a mean of 250 milliseconds with a standard deviation of 40 milliseconds. The shape of this population's distribution is unknown. A biologist randomly selects a sample of 50 frogs.
1. What is the probability that a single frog, chosen at random, reacts in less than 235 milliseconds?
2. Check that the Central Limit Theorem applies here, then find the probability that the mean reaction time of the sample of 50 frogs is less than 235 milliseconds.

### Solution

**Part 1: Single frog**

$$\mu = 250 \qquad \sigma = 40$$

$$z = \frac{x-\mu}{\sigma} = \frac{235-250}{40} = \frac{-15}{40} = -0.38$$

$$P(x < 235) = P(z < -0.38) = 0.3520 = \mathbf{35.20\%}$$

There is about a 35.20% chance that a single, randomly-chosen frog reacts in less than 235 milliseconds.

**Part 2: Sample of 50 frogs**

Check the conditions for the Central Limit Theorem:
* __Is the sample randomly selected?__ Yes, the problem states the sample of 50 frogs is random.
* __Is the sample large enough?__ Our sample size is $n=50$, which *is* larger than 30. This condition is satisfied on its own - we don't need to know anything about the shape of the population distribution, which is good, because the problem tells us it's unknown!

Since both conditions are satisfied, the Central Limit Theorem applies.

$$\mu_{\bar{x}} = \mu = 250 \qquad \sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{40}{\sqrt{50}} = \frac{40}{7.071} = 5.657$$

$$z = \frac{\bar{x}-\mu_{\bar{x}}}{\sigma_{\bar{x}}} = \frac{235-250}{5.657} = \frac{-15}{5.657} = -2.65$$

$$P(\bar{x} < 235) = P(z < -2.65) = 0.0040 = \mathbf{0.40\%}$$

**Comparison:** A single frog has about a 35.20% chance of reacting in less than 235 milliseconds, but the average reaction time of a random sample of 50 frogs has only about a 0.40% chance of being that fast. Notice that here, we were able to use the Central Limit Theorem even though we don't know the shape of the population distribution - because our sample size of 50 is larger than 30.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_4_Example.html#practice)
