<head>
<title>Lesson 7.1 Variance</title>
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

# Lesson 7.1 Variance
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 2.2.2 Standard deviation as a measure of spread (pages 58-61)

## Lesson
To measure the spread, we want to see how far the points are from the center. To do this, we use the __deviation__.

$$x-\bar{x}\tag{Deviation}$$

Once we have the deviations for all the points, we could take an average. However, the average of all these deviations will be 0. This is because the mean is the middle point, so there are equal deviations above and below the mean, giving an average of 0. How do we fix this? We square the deviations.

$$(x-\bar{x})^2\tag{Squared Deviation}$$

Now, we can take the average. This average is known as the __variance__ and is the primary tool used for determining how spread out the data is. Taking the average for a population is straightforward. However, the average for a sample has one difference: we divide by $(n-1)$.

$$\sigma^2 = \frac{\sum (x-\mu)^2}{n}\tag{Variance of a Population}$$

$$s^2 = \frac{\sum (x-\bar{x})^2}{n-1}\tag{Variance of a Sample}$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/HxcSVjm6p80?si=XP47XRoiPdspmMik" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
Calculate the variance for each of the questions below. First, solve it by hand, check the solution, then try it on the calculator.

1. The ages of all 6 employees at a small office are: \[24, 28, 22, 30, 26, 26\]. Since this is every employee at the office, treat this as a **population**. Find the population variance.
  - [After solving on your own, see solution here](./Solutions/7_1_Solution1.html)
2. A researcher weighs a **sample** of 5 puppies from a large litter: \[8, 10, 9, 11, 12\] pounds. Find the sample variance.
  - [After solving on your own, see solution here](./Solutions/7_1_Solution2.html)
3. Two vending machines are each timed on 5 separate fills (in seconds):
  - Machine A: \[30, 32, 31, 29, 33\]
  - Machine B: \[25, 40, 20, 35, 30\]
  - Treating each list as a sample, find the sample variance for Machine A and for Machine B. Which machine is more consistent? Explain how the variance tells you this.
  - [After solving on your own, see solution here](./Solutions/7_1_Solution3.html)


<!--
## Technology

### TI-83/84

### Excel

### Desmos
-->