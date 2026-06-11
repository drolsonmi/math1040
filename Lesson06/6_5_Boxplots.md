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

# 6.5 Boxplots

## Resources
* [Desmos Demonstration of creating a boxplot](https://www.desmos.com/calculator/nz6r1pzy2p)

## Reading
* 2.2.3 Box plots and quartiles (pages 61-64)
* 2.2.5 Outliers and robust statistics (pages 66-68)

## Lesson
### Boxplots (or box-and-whisker plots)
A boxplot is a very simple graph intended to display the distribution of the quartiles. In order for the graph to be effective, we must start with the scale and the label:
1. Create a numberline that starts below your minimum and goes beyond your maximum
2. Label your numberline (what is the data that you are going to show)
3. Draw lines above the numberline at the locations of
    * The minimum
    * Q1 (1st Quartile)
    * The median
    * Q3 (3rd Quartile)
    * The maximum
4. Connect Q1 to Q3 to create a box (the median line will be inside the box, essentially dividing the box in two)
5. Draw a single line from the minimum to Q1 and another from Q3 to the maximum (these are the whiskers)

<iframe width="560" height="315" src="https://www.youtube.com/embed/2viqSRfP2Us?si=rmKKny7FWT5a0Srs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe src="https://www.desmos.com/calculator/nz6r1pzy2p?embed" width="500" height="300" style="border: 1px solid #ccc" frameborder=0></iframe>

### Interquartile Range
The __interquartile range__ (IQR) is the range between Q1 and Q3. In other words, it is the range of the box in our boxplot.

In short, *IQR = Q3 - Q1*.

### Outliers
Sometimes, our boxplot gets really long whiskers - ridiculously long whiskers. This is because we may have a single point that is ridiculously extreme one way or the other. 

There is a way to exclude these extreme points from the plot. Using the IQR, we can judge what a reasonable distance is to consider points valid or extreme. If points are within this distance, we keep them in the graph. Points beyond this reasonable distance are called __outliers__.

What is this reasonable distance? *Any point within $$1.5\cdot IQR$$ of the box is reasonable. Any points further than $$1.5\cdot IQR$$ from the box is considered an outlier.* In short, 
* Points above $$Q3 + 1.5IQR$$ are outliers
* Points between $$Q1 - 1.5IQR$$ and $$(Q3 + 1.5IQR)$$ are valid
* Points below $$(Q1 - 1.5IQR)$$ are outliers

<iframe width="560" height="315" src="https://www.youtube.com/embed/JpMn8y-Rfrs?si=mk9RpAwVJl7SikNN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


<!--
Perhaps it would be a good idea to create 6.6 Boxplots and Skewness (compare to histograms)


## Practice

## Technology

### TI-83/84

### Excel

### Desmos
-->