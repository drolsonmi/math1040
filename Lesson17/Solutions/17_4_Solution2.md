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
<title>Solution for practice 17.4.2</title>
</head>

## 17.4 Example - Solution for Practice 2
A cereal company's boxes are labeled as containing 16 ounces of cereal. The actual weight of cereal in each box is normally distributed with a mean of 16 ounces and a standard deviation of 0.5 ounces. A grocery store manager randomly selects a sample of 25 boxes.
1. What is the probability that a single box, chosen at random, weighs more than 16.3 ounces?
2. Check that the Central Limit Theorem applies here, then find the probability that the mean weight of the sample of 25 boxes is more than 16.3 ounces.

### Solution

**Part 1: Single box**

$$\mu = 16 \qquad \sigma = 0.5$$

$$z = \frac{x-\mu}{\sigma} = \frac{16.3-16}{0.5} = \frac{0.3}{0.5} = 0.60$$

$$P(x > 16.3) = P(z > 0.60) = 1 - 0.7257 = 0.2743 = \mathbf{27.43\%}$$

There is about a 27.43% chance that a single, randomly-chosen box weighs more than 16.3 ounces.

**Part 2: Sample of 25 boxes**

Check the conditions for the Central Limit Theorem:
* __Is the sample randomly selected?__ Yes, the problem states the sample of 25 boxes is random.
* __Is the sample large enough?__ Our sample size is only $n=25$, which is not larger than 30. However, the problem tells us that the weight of cereal in each box is normally distributed, so this condition is satisfied by the exception for normally-distributed populations.

Since both conditions are satisfied, the Central Limit Theorem applies.

$$\mu_{\bar{x}} = \mu = 16 \qquad \sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}} = \frac{0.5}{\sqrt{25}} = \frac{0.5}{5} = 0.1$$

$$z = \frac{\bar{x}-\mu_{\bar{x}}}{\sigma_{\bar{x}}} = \frac{16.3-16}{0.1} = \frac{0.3}{0.1} = 3.00$$

$$P(\bar{x} > 16.3) = P(z > 3.00) = 1 - 0.9987 = 0.0013 = \mathbf{0.13\%}$$

**Comparison:** A single box has about a 27.43% chance of weighing more than 16.3 ounces, but the average weight of a random sample of 25 boxes has only about a 0.13% chance of being that high. It is far less likely for the sample *average* to be unusually high than it is for any one individual box.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_4_Example.html#practice)
