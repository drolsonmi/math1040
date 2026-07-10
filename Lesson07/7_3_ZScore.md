<head>
<title>Lesson 7.3 The Z-Score</title>
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

# Lesson 7.3 The Z-Score
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 4.1.2 Standardizing with Z-scores (pages 142-143)

## Lesson
The z-score is, in essence, the number of standard deviations a given value is from the mean.

We can easily go from the value to the z-score with the following equation:

$$z=\frac{x-\bar{x}}{s}\tag{Z-Score}$$

Here are a few things we can learn from a z-score:
- A **positive** z-score means the value is *above* the mean.
- A **negative** z-score means the value is *below* the mean.
- A z-score of **0** means the value *is* the mean.
- The **farther** a z-score is from 0 (in either direction), the farther that value is from the mean, in units of standard deviation. A z-score of 2 is twice as many standard deviations from the mean as a z-score of 1.

### How Z-Scores Are Used
Imagine you have two completely different distributions. If you want to compare values from both distributions, that will be hard since they are on different scales. Z-scores are useful because they take a value out of its original units and place it on a common, standardized scale. This makes it possible to do things that would otherwise be difficult or meaningless:
 
1. __Comparing values from different distributions.__
- Suppose one student scores 88 on a test with a mean of 80, and a friend scores 91 on a *completely different* test with a mean of 85. You can't compare 88 and 91 directly — they came from different tests, with different means and different spreads. But if you convert each score to a z-score, you're now comparing both students on the same scale: "how many standard deviations above their own test's average did they score?" Whichever z-score is higher represents the *relatively* stronger performance, even though the raw scores themselves aren't directly comparable.
 
2. __Identifying unusual values or possible outliers.__
- Since a z-score tells you how many standard deviations a value is from the mean, it gives us a quick way to flag values that are unusually far from the rest of the data. As a rough guideline, a value with $|z| > 2$ is often considered somewhat unusual, and a value with $|z| > 3$ is often considered a likely outlier. We'll make this more precise in the next lesson when we cover the Empirical Rule.
 
3. __Working backward from a z-score to a data value.__
- The z-score formula can be rearranged to solve for $x$ instead of $z$:
 
  $$x = \bar{x} + z\cdot s$$
 
- This lets us answer questions in the other direction — for example, "what score would a student need in order to be exactly 1.5 standard deviations above the mean?" — without needing to know the original raw data.
 
4. __Laying the groundwork for working with the normal distribution.__
- In future lessons, z-scores will become the key tool for finding probabilities and percentiles under the normal distribution. Every normal distribution has a different mean and standard deviation, but once a value is converted to a z-score, it can be compared to the same standard normal distribution every time.

<iframe width="560" height="315" src="https://www.youtube.com/embed/5TNR-RB2EMg?si=f7KigbkK5G9wXfBR" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. A student scores 82 on a test. The class mean was 75, with a standard deviation of 5. Find the student's z-score.
  - [After solving on your own, see solution here](./Solutions/7_3_Solution1.html)
2. Sally scores 88 on Test A, where the mean was 80 and the standard deviation was 4. Tom scores 91 on Test B, a completely different test, where the mean was 85 and the standard deviation was 2. Find each student's z-score, and determine who performed better relative to their own test.
  - [After solving on your own, see solution here](./Solutions/7_3_Solution2.html)
3. A dataset has a mean of 50 and a standard deviation of 8. What data value corresponds to a z-score of $-1.5$?
  - [After solving on your own, see solution here](./Solutions/7_3_Solution3.html)
