<head>
<title>Lesson 7.4 The Empirical Rule</title>
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

# Lesson 7.4 The Empirical Rule
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 2.2.2 Standard deviation as a measure of spread (pages 58-61)

## Lesson
We've now spent this lesson building tools to measure spread: the variance, the standard deviation, and the z-score. The **Empirical Rule** ties all of these together and gives us a fast, practical way to describe *how much* of a dataset falls within a certain distance of the mean — but only when the data has a specific shape.
 
### When Does the Empirical Rule Apply?
 
The Empirical Rule only applies to data that is **unimodal and roughly symmetric** — that is, data whose histogram forms a rough bell shape, with one peak in the middle and the two sides mirroring each other. This is often called an approximately **normal distribution**. If a distribution is heavily skewed, has multiple peaks, or has major outliers, the Empirical Rule does **not** apply, and the percentages below will not be accurate.
 
### The Rule Itself
 
For data that is approximately normal, the Empirical Rule (sometimes called the **68-95-99.7 Rule**) states:
 
- About **68%** of the data falls within **1 standard deviation** of the mean: $(\bar{x} - s, \ \bar{x} + s)$
- About **95%** of the data falls within **2 standard deviations** of the mean: $(\bar{x} - 2s, \ \bar{x} + 2s)$
- About **99.7%** of the data falls within **3 standard deviations** of the mean: $(\bar{x} - 3s, \ \bar{x} + 3s)$

Notice that this connects directly back to the z-score: a value with $z = 1$ sits right at the edge of the 68% region, a value with $z=2$ sits at the edge of the 95% region, and a value with $z=3$ sits at the edge of the 99.7% region. In fact, one of the most useful applications of the Empirical Rule is estimating just how *unusual* a value is once you know its z-score — a value with $|z| > 2$ is already outside the middle 95% of the data, and a value with $|z| > 3$ is extremely rare.
 
![The Empirical Rule](https://drolsonmi.github.io/math1040/Lesson07/images/Fig741_EmpiricalRule.png)
 
### Using Symmetry to Find the Tails
 
Because a normal distribution is symmetric, we can use the 68-95-99.7 percentages to figure out the percentage of data in *any* one of the eight labeled regions above, not just the three "middle" regions.
 
For example, since 68% of the data falls within 1 standard deviation of the mean, the remaining $100\% - 68\% = 32\%$ must be split evenly between the two tails (below $\bar{x}-s$ and above $\bar{x}+s$), because the distribution is symmetric:
 
$$\frac{100\% - 68\%}{2} = \frac{32\%}{2} = 16\%$$
 
So about 16% of the data lies more than 1 standard deviation *above* the mean, and about 16% lies more than 1 standard deviation *below* the mean.
 
We can use this same idea to find the percentage of data between any two of the marked standard deviation lines. For example, the percentage of data between 1 and 2 standard deviations above the mean is found by subtracting the inner region from the outer region, then dividing by 2 (since both sides are identical):
 
$$\frac{95\% - 68\%}{2} = \frac{27\%}{2} = 13.5\%$$
 
This is exactly where the 13.5% labels in the diagram above come from.
 
### Why the Empirical Rule Matters
 
The Empirical Rule gives us a quick way to:
 
- Estimate what proportion of a dataset falls within a given range, without needing raw data or a calculator
- Identify how unusual a specific value is, by combining it with a z-score
- Build intuition for the normal distribution before we study it formally later in the course, since the percentages here are just a preview of the areas we'll calculate more precisely under the normal curve

<iframe width="560" height="315" src="https://www.youtube.com/embed/rvMb72Tw9js?si=iWBBm_LZNXXH8RFm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
 
Assume all datasets below are approximately normally distributed.
 
1. The lifespans of a certain type of light bulb are approximately normal, with a mean of 1200 hours and a standard deviation of 50 hours. Between what two values do about 68% of the light bulbs' lifespans fall?
  - [After solving on your own, see solution here](./Solutions/7_4_Solution1.html)
2. Using the same light bulb data (mean = 1200 hours, standard deviation = 50 hours), estimate the percentage of light bulbs that last **less than 1100 hours**.
  - [After solving on your own, see solution here](./Solutions/7_4_Solution2.html)
3. Using the same light bulb data (mean = 1200 hours, standard deviation = 50 hours), estimate the percentage of light bulbs that last **between 1250 and 1300 hours**.
  - [After solving on your own, see solution here](./Solutions/7_4_Solution3.html)

