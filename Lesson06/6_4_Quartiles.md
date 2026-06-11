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

# 6.4 Quartiles

## Reading
* 2.2.3 Box plots and quartiles (pages 61-64)
* 2.2.4 Calculator: summarizing 1-variable statistics (pages 64-66)

## Lesson
### Quartiles
The median cut the dataset in half to find the middle of the data. Quartiles cut the dataset into quarters.
* Find the median (cuts the dataset in half)
* Find the median of each half (cuts the datset into quarters) - we'll call these values __quartiles__.

The __1st quartile__ is the value separating the lowest (and first) quarter of the data from the second quarter.

The __2nd quartile__ is the value separating the second quarter from the third. *Note that this is also the median.*

The __3rd quartile__ is the value separating the third quarter from the fourth.


### The 5-number Summary
When we separated the data into quarters, we created 5 values that describe the data. We call these values the __5-number Summary__. The 5 numbers are:
* Minimum (value before the 1st quarter of the data)
* 1st Quartile (Q1) (value between 1st and 2nd quarters)
* Median (also 2nd quartile, value between 2nd and 3rd quarters)
* 3rd Quartile (Q3) (value between 3rd and 4th quarters)
* Maximum (value after the 4th quarter of the data)

When finding the 5-number summary, it is helpful to:
1. Create a table:

 | Minimum |  Q1   | Median |  Q3   | Maximum |
 | :-----: | :---: | :----: | :---: | :-----: |
 |         |       |        |       |         |

2. Identify the Minimum and the Maximum
3. Find the Median
4. Find the Quartiles

(These are not required steps, but if you are struggling, they are good steps to get started.)

<iframe width="560" height="315" src="https://www.youtube.com/embed/cPsIzs5dOdw?si=Je_UhmdlXX9n9dqD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Percentiles
Percentiles are very similar to quartiles. 

| Quartiles | Percentiles | 
| :-------- | :---------- |
| Quartiles divide the data into quarters. | Percentiles divide the data into cents (meaning into hundredths). |
| The 1st quartile is where you are above the lowest quarter of the data.<br>The 3rd quartile is where you above the lowest three quarters of the data. | The 32th percentile is where you are above the lowest 32\% of the data.<br>The 94th percentile is where you are above the lowest 94\% of the data. |

There are some common points between quartiles and percentiles. For example,
* The 1st quartile separates the lowest quarter (or 25\%) of the data ==> 25th percentile
* The median separates half (or 50\%) of the data ==> 50th percentile
* The 3rd quartile separates the lowest three quarters (or 75\%) of the data ==> 75th percentile

In this class, this is about as far as we need to go with percentiles. They are very useful and you should have a basic understanding of them. But we are only going to work with quartiles in this class.

## Practice

## Technology
There are a few different ways to calculate quartiles. Different software calculates the quartiles differently. The method we learned here is the method used by the TI-83/TI-84. However, it is useful to see how it is done with other technologies.

For homework and exams, we will stick with the TI-84 method as we learned. So if you have a different calculator, then be sure you know how to do this method by hand.

### TI-83/84
<iframe width="560" height="315" src="https://www.youtube.com/embed/CSyY_vLoM7Q?si=RzNNN_pf2_gy07V-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Excel
Excel does not calculate quartiles like we did in class. It interpolates between values, then finds the 25th percentile. For example, if your dataset is {0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10}, then
* Excel will add values between these values to give us 100 points:
  * {0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9, 2, 2.1, 2.2, ..., 9.8, 9.9, 10}
* Excel will then find the 25th percentile, which in this case would be 2.5

It is important to be aware of this as these results may differ from the results of a TI-84.

There are 3 different functions
* `=quartile.inc([array],[quartile])`
    * Includes the minimum and the median to find Q1
    * Includes the median and the maximum to find Q3
* `=quartile.exc([array],[quartile])`
    * Excludes the minimum and the median to find Q1
    * Excludes the median and the maximum to find Q3
* `=quartile([array],[quartile])`
    * Follows the `quartile.exc` calculation

### Desmos
