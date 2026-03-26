<head>
<title>19.2 Confidence Interval for a Proportion</title>
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

# Lesson 19.2 Confidence Interval for a Proportion
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.1.1 Confidence intervals for a proportion (pages 218–222)

## Lesson
To find a confidence interval for a proportion, follow these steps:
1. Verify the Central Limit Theorem applies (If it doesn't apply, we can't solve the problem)
2. Find the Critical Value
3. Find the Margin of Error
4. Find the Confidence Interval
5. Interpret the Confidence Interval

Let's work through the same scenario from Lesson 19.1:

> A local college wants to estimate the true proportion of its students who work a part-time job. A random sample of 200 students is taken, and 130 of them report working part-time. What is the true proportion of students at this college who work part-time?

We'll find a 95% confidence interval. As we did in Lesson 18.3, we walk through all five steps.

#### 1. Verify the Central Limit Theorem
These are the two requirements needed to satisfy the Central Limit Theorem for proportions:
1. __The sample must be random__
    * The problem states that the sample is random, so *this is satisfied*
2. __The sample must be large enough__
    * Since we are dealing with categorical data and proportions, we require $n\hat{p} \ge 10$ and $n\hat{q} \ge 10$
    * First, compute the sample proportion: 

        $$\hat{p} = \frac{x}{n} = \frac{130}{200} = 0.65$$
        $$\hat{q} = 1 - \hat{p} = 0.35$$

    * $n\hat{p} = 200(0.65) = 130 \ge 10$ — *this is satisfied*
    * $n\hat{q} = 200(0.35) = 70 \ge 10$ — *this is satisfied*

Since __both__ conditions are satisfied, __the Central Limit Theorem passes, and we can continue with this problem__.

#### 2. Find the Critical Value
We are given a confidence level of 95%.
* The remaining 5% is in the two tails, 2.5% in each tail
* The z-scores that separate the two tails are $z_c = \pm 1.96$

#### 3. Find the Margin of Error
The equation for the margin of error for a proportion is 

$$E = z_c\sqrt{\tfrac{\hat{p}\hat{q}}{n}} = z_c\sqrt{\tfrac{\hat{p}(1-\hat{p})}{n}}$$

* $z_c = 1.96$ is the critical value
* $\hat{p} = 0.65$ is the sample proportion
* $\hat{q} = 0.35$ is the complement of the sample proportion
* $n = 200$ is the sample size

Plugging these in,

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} = z_c\sqrt{\tfrac{\hat{p}(1-\hat{p})}{n}} \\
  &= 1.96\sqrt{\frac{(0.65)(0.35)}{200}} \\
  &= 1.96\sqrt{\frac{0.2275}{200}} \\
  &= 1.96 \times 0.03373 \\
  &\approx \mathbf{0.066}
\end{align*}$$

#### 4. Find the Confidence Interval
The boundaries of the confidence interval are the sample proportion ($\hat{p}$) plus or minus the margin of error ($E$).
* $\hat{p} = 0.65$ is the sample proportion
* $E = 0.066$ is the margin of error

$$\hat{p} + E = 0.65 + 0.066 = 0.716$$

$$\hat{p} - E = 0.65 - 0.066 = 0.584$$

The confidence interval is,

$$\mathbf{(0.584,\ 0.716)}$$

#### 5. Interpret the Confidence Interval
The goal was to find the true proportion of students who work part-time. Although we couldn't find an exact value, we found the confidence interval — a range of values in which the true proportion is likely to fall.

Here is a proper interpretation of the confidence interval:

> __We are 95% confident that the true proportion of students at this college who work a part-time job is between 0.584 and 0.716 (between 58.4% and 71.6%).__

Notice that it is common and natural to express the confidence interval as percentages when the variable is a proportion or a percentage.

## Practice
1. A local news station surveys a random sample of 300 residents and finds that 174 support a proposed new park. Construct a 95% confidence interval for the true proportion of residents who support the new park.
    * [After solving on your own, see solution here](Solutions/19_2_Solution1.md)

2. A quality control inspector at a factory randomly selects 500 items off the assembly line and finds that 45 are defective. Construct a 99% confidence interval for the true proportion of defective items produced by this factory.
    * [After solving on your own, see solution here](Solutions/19_2_Solution2.md)

3. A university researcher surveys a random sample of 180 students and finds that 63 report experiencing high levels of stress during finals week. Construct a 90% confidence interval for the true proportion of students who experience high stress during finals week.
    * [After solving on your own, see solution here](Solutions/19_2_Solution3.md)

## Technology
### TI-83/84
To calculate the Confidence Interval for a proportion on a TI-83/84,
* Press `STAT`
* Select the `TESTS` menu
* Select `A:1-PropZInt...`
* Enter $$x$$ (number of successes), $$n$$ (sample size), and the confidence level (C-Level)
* Select "Calculate"

The calculator will display the confidence interval bounds, the sample proportion $$\hat{p}$$, and the sample size $$n$$. You can verify your margin of error by computing half the width of the interval:

$$E = \frac{\text{Upper Bound} - \text{Lower Bound}}{2}$$

### Desmos
To compute the confidence interval in [Desmos](www.desmos.com/calculator), you can calculate the margin of error directly and add/subtract it from $$\hat{p}$$:

* Lower bound: $$\hat{p} - z_c\sqrt{\tfrac{\hat{p}\hat{q}}{n}}$$
* Upper bound: $$\hat{p} + z_c\sqrt{\tfrac{\hat{p}\hat{q}}{n}}$$

For example, for the practice problem above with $$\hat{p} = 0.65$$, $$n = 200$$, and $$z_c = 1.96$$, type:

$$0.65 - 1.96\sqrt{\frac{0.65 \times 0.35}{200}}$$

and

$$0.65 + 1.96\sqrt{\frac{0.65 \times 0.35}{200}}$$

Replace the values with those from your specific problem.