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
<title>Solution for practice 17.4.1</title>
</head>

## 17.4 Example - Solution for Practice 1
A brand of batteries has a mean lifetime of 500 hours with a standard deviation of 50 hours. The lifetime of these batteries follows a normal distribution. A quality control inspector randomly selects a sample of 9 batteries.
1. What is the probability that a single battery, chosen at random, lasts less than 460 hours?
2. Check that the Central Limit Theorem applies here, then find the probability that the mean lifetime of the sample of 9 batteries is less than 460 hours.

### Solution

**Part 1: Single battery**

$$\mu = 500 \qquad \sigma = 50$$

$$z = \frac{x-\mu}{\sigma} = \frac{460-500}{50} = \frac{-40}{50} = -0.80$$

$$P(x < 460) = P(z < -0.80) = 0.2119 = \mathbf{21.19\%}$$

There is about a 21.19% chance that a single, randomly-chosen battery lasts less than 460 hours.

**Part 2: Sample of 9 batteries**

First, check the conditions for the Central Limit Theorem:
* __Is the sample randomly selected?__ Yes, the problem states the sample of 9 batteries is random.
* __Is the sample large enough?__ Our sample size is only $n=9$, which is not larger than 30. However, the problem tells us that battery lifetime follows a normal distribution, so this condition is satisfied by the exception for normally-distributed populations.

Since both conditions are satisfied, the Central Limit Theorem applies.

$$\mu_{\bar{x}} = \mu = 500 \qquad \sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{50}{\sqrt{9}} = \frac{50}{3} = 16.667$$

$$z = \frac{\bar{x}-\mu_{\bar{x}}}{\sigma_{\bar{x}}} = \frac{460-500}{16.667} = \frac{-40}{16.667} = -2.40$$

$$P(\bar{x} < 460) = P(z < -2.40) = 0.0082 = \mathbf{0.82\%}$$

**Comparison:** A single battery has about a 21.19% chance of lasting less than 460 hours, but the average of a random sample of 9 batteries has only about a 0.82% chance of being that low. This matches what we'd expect - it's much less likely for the *average* of several batteries to be unusually low than it is for any one individual battery.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_4_Example.html#practice)
