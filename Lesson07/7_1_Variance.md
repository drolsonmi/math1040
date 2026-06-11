<head>
<!--<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>-->
<script src="https://cloudflare.com" integrity="sha512-bb9v9wun86lzgQv5w0w6gO89W74U5C4lFvP6gL7P3hZ9M4A6fC0hB4Zg4m9o2F4P5C6b8F9G0H1I2J3K4L5M6== " crossorigin="anonymous" referrerpolicy="no-referrer"></script>
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

Now, we can take the average. This average is known as the __variance__ and is the primary tool used for determining how spread out the data is. Taking the average for a population is straightforward. However, the average for a sample has one difference: we divide by $$n-1$$.

$$\sigma^2 = \frac{\sum (x-\mu)^2}{n}\tag{Variance of a Population}$$

$$s^2 = \frac{\sum (x-\bar{x})^2}{n-1}\tag{Variance of a Sample}$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/HxcSVjm6p80?si=XP47XRoiPdspmMik" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<!--
## Practice


1. ?
    * After solving on your own, check the <button popovertarget="Problem_1">Solution</button>
2. ?
    * After solving on your own, check the <button popovertarget="Problem_2">Solution</button>
3. ?
    * After solving on your own, check the <button popovertarget="Problem_3">Solution</button>

<div popover id="Problem_1">

## Problem 20.1.1
A popover is an element that is placed on top of everything else.
* Item 1
* Item 2

$$\bar{x}=\frac{1}{n}\sum x$$
It can be used when you want to tell something important.

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

## Problem 20.1.2
A popover is an element that is placed on top of everything else.
* Item 1
* Item 2

$$\bar{x}=\frac{1}{n}\sum x$$
It can be used when you want to tell something important.

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

## Problem 20.1.3
A popover is an element that is placed on top of everything else.
* Item 1
* Item 2

$$\bar{x}=\frac{1}{n}\sum x$$
It can be used when you want to tell something important.

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>
-->

<!--
## Technology

### TI-83/84

### Excel

### Desmos
-->