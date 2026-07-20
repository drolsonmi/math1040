<head>
<title>Lesson 15.3 Probability from a Normal Distribution</title>
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

# Lesson 15.3 Probability from a Normal Distribution
## Reading

Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)

- 4.1.3 Normal probability table (pages 143-144)
- 4.1.4 Normal probability examples (pages 144-147)
- 4.1.5 Calculator: finding normal probabilities (pages 148-150)
- 4.1.6 68-95-99.7 rule (page 150)

## Lesson

A **Z-Table** is a convenient tool that helps us to calculate the area to the left of a z-score. Remember that *area = probability*, so by finding the area to the left of a z-score, we are finding the probability of randomly getting a value less than that z-score.

The Z-Table *always* gives us the area to the LEFT of the z-score. This area can also be found on a calculator. Unless it gives you the option to tell otherwise, it will also give you the area to the LEFT. (I have videos on finding the areas using a TI-84 below. I have also included a video on how to do this with Desmos below if desired.)

[https://www.youtube.com/embed/yWhPWzh1vL4?si=8WirIj1SR9-xKUX0](https://www.youtube.com/embed/yWhPWzh1vL4?si=8WirIj1SR9-xKUX0)

If the Z-Table only gives the area to the LEFT ($P(z < z_c)$), then how do you find the area to the RIGHT ($P(z > z_c)$)?

Recall that the total area under the normal curve is 1.0. So, $P(z < z_c) + P(z > z_c) = 1.0$. That means the two sides of the normal curve are complements of each other. In other words,

$$P(z > z_c) = 1.0 - P(z < z_c)$$

[https://www.youtube.com/embed/l85wo0hJRTU?si=ZTghJ439wr0xUSbp](https://www.youtube.com/embed/l85wo0hJRTU?si=ZTghJ439wr0xUSbp)

In both of these examples, we have looked at how to find the areas of the tails. What if we want the area of a middle section? That is, what if we want $P(a < z < b)$? There are two methods:

### Method 1: Remove the two tails

Remember that the entire area equals 1.0. If we remove the tail to the right of $b$ ($P(z > b)$, depicted in green in the figure below), and the tail to the left of $a$ ($P(z < a)$, depicted in blue in the figure below), then we'll only be left with the area in the middle ($P(a < z < b)$, depicted in red in the figure below).

![Removing the two tails to find the middle area](https://drolsonmi.github.io/math1040/Lesson15/images/remove_two_tails.png)

### Method 2: Remove the left tail

We can start with the area left of $b$, which is $P(z < b)$. However, this also includes the left tail, which is $P(z < a)$ (depicted in blue in the figure below). We don't want to include this area. So, we can just remove it. This will leave us just the area between $a$ and $b$, which is $P(a < z < b)$, depicted in red in the figure below.

![](https://drolsonmi.github.io/math1040/Lesson15/images/remove_one_tail.png "Removing the left tail to find the middle area")

[https://www.youtube.com/embed/RRFJZDXrg6o?si=2dYUvevhMHb620hN](https://www.youtube.com/embed/RRFJZDXrg6o?si=2dYUvevhMHb620hN)

## Technology

### TI-83/84

[https://www.youtube.com/embed/J1WImZgnBDY?si=JYl8eQmOYtKv3B1o](https://www.youtube.com/embed/J1WImZgnBDY?si=JYl8eQmOYtKv3B1o)

### Excel

In Microsoft Excel, the `NORM.DIST` function finds the area to the LEFT of a given value in a normal distribution.

- Type `=NORM.DIST(` then enter, in order: the value $x$, the mean, the standard deviation, and `TRUE` (this tells Excel to give the cumulative area to the left rather than just the height of the curve)
  * For example, `=NORM.DIST(220,210,10,TRUE)` finds $P(x < 220)$ for a distribution with mean 210 and standard deviation 10
- Close the parenthesis and press `Enter`
- If you already have a z-score instead of a raw value, use `=NORM.S.DIST(` followed by the z-score and `,TRUE)` instead
  * For example, `=NORM.S.DIST(-1.5,TRUE)` finds $P(z < -1.5)$
- Since Excel always gives the area to the LEFT, find the area to the RIGHT by subtracting from 1: `=1-NORM.DIST(x,mean,standard_dev,TRUE)`
- Find the area of a middle section between two values by subtracting the smaller cumulative area from the larger one: `=NORM.DIST(upper,mean,standard_dev,TRUE)-NORM.DIST(lower,mean,standard_dev,TRUE)`

### Desmos

[https://www.youtube.com/embed/pfJ1TZx2YGw?si=owZAZYEx_iB1zdcW](https://www.youtube.com/embed/pfJ1TZx2YGw?si=owZAZYEx_iB1zdcW)

## Practice

1. A tire manufacturer finds that the lifespan of their tires is approximately normally distributed with a mean of 50,000 miles and a standard deviation of 4,000 miles. Find the probability that a randomly selected tire lasts **less than 45,000 miles**.
  - [After solving on your own, see solution here](./Solutions/15_3_Solution1.html)
2. Using the same tire data (mean = 50,000 miles, standard deviation = 4,000 miles), find the probability that a randomly selected tire lasts **more than 58,000 miles**.
  - [After solving on your own, see solution here](./Solutions/15_3_Solution2.html)
3. Package weights at a shipping center are approximately normally distributed with a mean of 50 lbs and a standard deviation of 3 lbs. Find the probability that a randomly selected package weighs **between 45 and 53 lbs**.
  - [After solving on your own, see solution here](./Solutions/15_3_Solution3.html)
4. Daily commute times for employees at a company are approximately normally distributed with a mean of 32 minutes and a standard deviation of 6 minutes. Find the probability that a randomly selected employee's commute is **between 20 and 44 minutes**, and compare your result to what the Empirical Rule would predict.
  - [After solving on your own, see solution here](./Solutions/15_3_Solution4.html)
