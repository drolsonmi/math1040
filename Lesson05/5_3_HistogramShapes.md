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

<!--
Ideas for practice questions:
* Show a graph and ask about the skew and what this means about the mean, median, and mode
* Give data. Ask student to graph it and then describe the skew
-->

# Lesson 5.3 Histogram Shapes

## Reading

Reading sections are from the [Introductory Statistics Textbook](https://drolsonmi.github.io/math1040/Resources/OpenIntroTextbook.pdf)

- 2.1.4 Describing Shape (pages 954-55)

## Lesson

<iframe width="560" height="315" src="https://www.youtube.com/embed/NY5cJC10EdY?si=g1R-qmAIrSeehH0v" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

One of the biggest advantages of a histogram is that it lets us see the overall **shape** of our data at a glance. This shape can tell us a lot about the story behind our data, and later in the course (when we get to Units 2 and 3) the shape will actually help us decide which statistical tools are appropriate to use. For now, let's focus on being able to recognize and describe four common shapes: **symmetric (normal)**, **skewed**, **uniform**, and **bimodal**.

### Symmetric / Normal Shape

A histogram is **symmetric** if you could fold it in half down the middle and the two sides would roughly match. When a symmetric histogram is also mound-shaped - low on both ends, building up to a single peak in the middle - we call this a **normal** (or bell-shaped) distribution. This is one of the most important shapes in all of statistics, and we will spend a lot of time with it in later lessons.

![Symmetric histogram of 0-60mph acceleration time](https://drolsonmi.github.io/math1040/Lesson05/images/Fig5_3_Normal.png)

In a symmetric, mound-shaped histogram, most of the data clusters near the center, with roughly equal numbers of datapoints tapering off toward each side.

### Skewed Distributions

Not every histogram is symmetric. Sometimes one side has a longer "tail" than the other. We call this a **skewed** distribution, and we name the skew based on which direction the *tail* points (not which side has the taller bars).

**Skewed Right (Positively Skewed):** Most of the data is bunched up on the low end, with a tail stretching out toward the higher values.

![Right-skewed histogram of horsepower](https://drolsonmi.github.io/math1040/Lesson05/images/Fig5_3_SkewedRight.png)

Horsepower is a good real-world example of this. Most cars have a fairly modest amount of horsepower, but a handful of high-performance cars stretch the tail out to the right.

**Skewed Left (Negatively Skewed):** Most of the data is bunched up on the high end, with a tail stretching out toward the lower values.

![Left-skewed histogram of quiz scores](https://drolsonmi.github.io/math1040/Lesson05/images/Fig5_3_SkewedLeft.png)

An easy quiz is a good example of this shape. Most students score well, clustered near the top, but a small number of students who struggled pull a tail out toward the lower scores.

> ***Memory Trick:*** Think of the tail like an arrow pointing in the direction of the skew. If the tail points right (toward the larger numbers), it's skewed right. If the tail points left (toward the smaller numbers), it's skewed left.

### Uniform Shape

A histogram is **uniform** when every bin has roughly the same frequency. Instead of a peak or a tail, the graph looks relatively flat across its entire width.

![Uniform histogram of cars by model year](https://drolsonmi.github.io/math1040/Lesson05/images/Fig5_3_Uniform.png)

The number of cars sampled from each model year in our dataset is a good example. Since roughly the same number of cars were sampled from each year between 1970 and 1982, no single bin dominates the graph.

### Bimodal (and Multimodal) Shapes

A histogram is **bimodal** when it has two distinct peaks, usually separated by a dip in the middle. This shape is a signal that you may actually be looking at *two different groups* combined into a single dataset.

![Bimodal histogram of adult heights](https://drolsonmi.github.io/math1040/Lesson05/images/Fig5_3_Bimodal.png)

Adult height is a classic example: if you combine the heights of men and women into a single sample, you tend to see two peaks - one for each group's typical height - rather than one single peak. If a histogram has more than two peaks, we call it **multimodal**.

### Why Shape Matters

Recognizing shape isn't just an exercise in vocabulary. The shape of your data hints at the story behind it:

- A skewed shape might mean there are unusually high or low values (sometimes called outliers) pulling the tail out
- A bimodal shape might mean your sample is really a mix of two different populations that should be studied separately
- A symmetric, mound shape suggests your data may follow a normal distribution, which unlocks many of the statistical tools we'll use starting in Unit 2

As you look at histograms throughout this course (and in the real world), get in the habit of asking: is it symmetric or skewed? Does it have one peak, two peaks, or no clear peak at all? These questions will become second nature with practice.

## Practice

1. For each histogram below, identify whether the shape is symmetric (normal), skewed right, skewed left, uniform, or bimodal.

    **Graph A:**

    <img src="https://drolsonmi.github.io/math1040/Lesson05/images/Fig531_PracticeA.png" width=450>

    **Graph B:**

    <img src="https://drolsonmi.github.io/math1040/Lesson05/images/Fig531_PracticeB.png" width=450>

    **Graph C:**

    <img src="https://drolsonmi.github.io/math1040/Lesson05/images/Fig531_PracticeC.png" width=450>

    **Graph D:**

    <img src="https://drolsonmi.github.io/math1040/Lesson05/images/Fig531_PracticeD.png" width=450>

- [After answering these questions on your own, check the solution](https://drolsonmi.github.io/math1040/Lesson05/Solutions/5_3_Solution1.html)

2. A real estate agent creates a histogram of home sale prices in a large city. Would you expect this histogram to be symmetric, skewed right, or skewed left? Explain your reasoning.
  - [After answering this question on your own, check the solution](https://drolsonmi.github.io/math1040/Lesson05/Solutions/5_3_Solution2.html)
