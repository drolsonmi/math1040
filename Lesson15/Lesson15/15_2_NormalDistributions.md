<head>
<title>Lesson 15.2 The Normal Distribution</title>
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

# Lesson 15.2 The Normal Distribution
## Reading

Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)

- 4.1.1 Normal distribution model (pages 141-142)
- 4.1.2 Standardizing with Z-scores (pages 142-143)

## Lesson

The **Normal Distribution** is the most important continuous distribution in statistics. Its density curve is the familiar bell-shaped curve: symmetric, single-peaked at the mean, and tapering off toward both tails. Many real-world variables — heights, blood pressure, standardized test scores, measurement errors — are approximately normal, which is part of why this distribution shows up so often.

[https://www.youtube.com/embed/JFZmA1nrpUU?si=NkyUXy1h9jrTaOQ_](https://www.youtube.com/embed/JFZmA1nrpUU?si=NkyUXy1h9jrTaOQ_)

### Area = Probability

Just like any density curve, the total area under a normal curve is exactly **1**. Since area under a density curve represents probability, this means:

- The area under the *entire* normal curve represents a probability of 1 (100%)
- The area under the curve between any two values $a$ and $b$ represents $P(a < X < b)$
- Because the curve is symmetric about the mean, exactly half (50%) of the area lies on each side of the mean

This is the whole reason we care about the normal distribution: once we know how to find areas under this curve, we can find the probability of *any* range of values.

### The Z-Score

Every normal distribution has its own mean ($\mu$) and standard deviation ($\sigma$), so a "high" value in one distribution might be an average value in another. To make normal distributions comparable — and to make it possible to use a single table or tool for all of them — we convert each value to a **z-score**, which tells us how many standard deviations a value is above or below the mean:

$$z=\frac{x-\mu}{\sigma}\tag{Z-Score}$$

- A **positive** z-score means the value is *above* the mean; a **negative** z-score means it is *below* the mean.
- Once a value has been converted to a z-score, it belongs to the **standard normal distribution**, which always has a mean of 0 and a standard deviation of 1. This is what lets us use one Z-table (or one calculator function) for every normal distribution, no matter its original mean or standard deviation.

[https://www.youtube.com/embed/e43uMhpKSOs?si=7QjCJb0BVb5Uq72t](https://www.youtube.com/embed/e43uMhpKSOs?si=7QjCJb0BVb5Uq72t)

### The Empirical Rule

For data that is approximately normal, the **Empirical Rule** (the 68-95-99.7 Rule) gives a quick way to estimate how much of the distribution falls within 1, 2, or 3 standard deviations of the mean:

- About **68%** of values fall within 1 standard deviation of the mean: $(\mu - \sigma, \ \mu + \sigma)$, i.e. $-1 < z < 1$
- About **95%** of values fall within 2 standard deviations of the mean: $(\mu - 2\sigma, \ \mu + 2\sigma)$, i.e. $-2 < z < 2$
- About **99.7%** of values fall within 3 standard deviations of the mean: $(\mu - 3\sigma, \ \mu + 3\sigma)$, i.e. $-3 < z < 3$

Notice that the Empirical Rule is really just a shortcut for the area under the curve at the specific z-scores $z = 1, 2,$ and $3$. In the next lesson, we'll learn how to find the area (probability) for *any* z-score, not just these three special cases.

## Practice

### Calculating Z-Scores

1. IQ scores are approximately normally distributed with a mean of $\mu = 100$ and a standard deviation of $\sigma = 15$. Find the z-score for a person with an IQ of 125.
  - [After solving on your own, see solution here](./Solutions/15_2_Solution1.html)
2. The heights of adult men are approximately normally distributed with $\mu = 69$ inches and $\sigma = 2.8$ inches. Find the z-score for a man who is 64 inches tall.
  - [After solving on your own, see solution here](./Solutions/15_2_Solution2.html)
3. Systolic blood pressure is approximately normally distributed with $\mu = 120$ and $\sigma = 12$. Find the z-score for a reading of 138, and interpret what this z-score means.
  - [After solving on your own, see solution here](./Solutions/15_2_Solution3.html)

### Using the Empirical Rule

Assume all distributions below are approximately normal.

4. Using the IQ distribution above ($\mu = 100$, $\sigma = 15$), between what two values do about 95% of IQ scores fall?
  - [After solving on your own, see solution here](./Solutions/15_2_Solution4.html)
5. Using the same IQ distribution, estimate the percentage of people with an IQ **above 130**.
  - [After solving on your own, see solution here](./Solutions/15_2_Solution5.html)
6. Using the height distribution above ($\mu = 69$ in, $\sigma = 2.8$ in), estimate the percentage of men **taller than 74.6 inches**.
  - [After solving on your own, see solution here](./Solutions/15_2_Solution6.html)
