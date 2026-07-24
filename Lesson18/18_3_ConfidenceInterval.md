<head>
<title>Confidence Interval when you know sigma</title>
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

# Lesson 18.3 Confidence Interval when you know $$\sigma$$
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 7.1.1 Using the z-distribution for inference when $\mu$ is unknown and $\sigma$ is known (pages 277)

## Lesson
To find a confidence interval, these are the steps you need to follow:
1. Verify the Central Limit Theorem applies (If it doesn't apply, we can't solve the problem)
2. Find the Critical Values
3. Find the Margin of Error
4. Find the Confidence Interval
5. Interpret the Confidence Interval

Let's apply what we have learned in a specific scenario. This is the problem we will work on:

> American mental abilities are often measured by an IQ test.  The IQ distribution is normal with a mean of 100 and a population standard deviation of 15.  
> 
> A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. What is the true average IQ of Snow College students?

We'll find a 90% confidence interval to find this true average. As we discussed, we need to do the following to find the confidence interval:

#### 1. Verify the Central Limit Theorem
These are the two requirements needed to satisfy the Central Limit Theorem:
1. __The sample must be random__
    * The problem states that the sample is random, so *this is satisfied*
2. __The sample must be large enough__
    * Since we are dealing with quantitative data and means, we want the sample to be at least 30
    * The sample size in the problem is $n=40$. Since $n\ge 30$, *this is satisfied*

Since __both__ conditions are satisfied, __the central limit theorem passes, and we can continue with this problem__.

#### 2. Find the Critical Values
We are given a confidence level of 90%.
* The remaining 10% is in the two tails, 5% in each tail
* The z-scores that separate the two tails are $$\pm$$1.645.

#### 3. Find the Margin of Error
The equation for the margin of error is $E = z_c\tfrac{\sigma}{\sqrt{n}}$.
* $z_c = \pm 1.645$ is the critical value
* $\sigma = 15$ is the population standard deviation
* $n = 40$ is the sample size

Plugging these in,
$$\begin{align*}
E &= z_c\frac{\sigma}{\sqrt{n}} \\
  &= \pm 1.645 \frac{15}{\sqrt{40}} \\
  &= \frac{\pm 24.675}{6.3246} \\
  &= \mathbf{3.90}
\end{align*}$$

#### 4. Find the Confidence Interval
The boundaries to our confidence interval are the sample mean ($$\bar{x}$$) plus or minus the margin of error ($$E$$).
* $\bar{x} = 106.3$ is the sample mean
* $E = 3.9$ is the standard error

$$\bar{x} + E = 106.3 + 3.9 = 110.20$$

$$\bar{x} - E = 106.3 - 3.9 = 102.4$$

The confidence interval is,

$$\mathbf{(102.4, 110.2)}$$

#### 5. Interpret the Confidence Interval
The goal was to find the true average IQ of Snow College students. Although we couldn't find an exact value, we can find the confidence interval, which is a range of values the true average could be in. So, we take this goal and apply it to the confidence interval we just found.

Here is a proper interpretation of the confidence interval:

> __We are 90% confident that the true average of Snow College student IQ scores is between the values of 102.4 and 110.2.__

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZwU7jF_qlkc?si=Jd7Y4uR1Fxu5evvC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

What if you are given a confidence interval. Can you find the margin of error? (Would I be asking if you couldn't?)

<iframe width="560" height="315" src="https://www.youtube.com/embed/UByp4S7E4bM?si=5jNSKuz2zkjm1f9u" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. A university is interested in estimating the average daily commute time for its students. A random sample of 50 students is selected, and their average commute time is found to be 32 minutes. The population standard deviation is known to be 8 minutes. Construct a 95% confidence interval for the true mean commute time of all students at the university.
    * [After solving on your own, see solution here](Solutions/18_3_Solution1.md)

2. A manufacturer claims that its LED light bulbs have an average lifespan of 1,200 hours. A consumer protection agency wants to verify this claim. They randomly select 40 bulbs and find that the sample has an average lifespan of 1,165 hours. The population standard deviation is known to be 100 hours. Construct a 99% confidence interval for the true mean lifespan of the manufacturer’s LED light bulbs.
    * [After solving on your own, see solution here](Solutions/18_3_Solution2.md)

3. A national education researcher wants to estimate the average SAT Math score for high school seniors in a particular state. A random sample of 60 students yields a sample mean score of 540. The population standard deviation is known to be 100 points. Construct a 92% confidence interval for the true mean SAT Math score of all high school seniors in the state.
    * [After solving on your own, see solution here](Solutions/18_3_Solution3.md)

## Technology
### TI-83/84
To calculate the Confidence Interval on a TI-83/84,
* Press `STAT`
* Select the `TESTS` menu
* Select `7:ZInterval...`
* Under "Inpt", select "Stats"
* Enter $$\sigma$$, $$\bar{x}$$, $$n$$, and the Confidence Level
* Select "Calculate"

<img src="images/Fig18_3a_TI84Input.png?raw=true" width="500" alt="TI-84 Confidence Interval Calculation"> <img src="images/Fig18_3b_TI84Results.png?raw=true" width="500" alt="TI-84 Confidence Interval Results">

Alternatively, you can put your data into a List, then under "Inpt" select "Data". Indicate the list your data is in, and it will calculate $$\bar{x}$$ and $$n$$ for you. (You will still need to indicate $$\sigma$$ and the confidence level.)

### Excel
To calculate the Confidence Interval in Excel,
1. Click on an empty cell where you want the margin of error to appear.
2. Type `=CONFIDENCE.NORM(alpha, sigma, n)` and press Enter, where:
    * `alpha` is 1 minus the confidence level, written as a decimal (for a 90% confidence level, alpha = 0.10)
    * `sigma` is the population standard deviation
    * `n` is the sample size
3. This returns the margin of error ($E$).
4. In two more cells, add and subtract $E$ from the sample mean ($\bar{x}$) to find the upper and lower boundaries of the confidence interval.
For example, with $\bar{x}=106.3$, $\sigma=15$, $n=40$, and a 90% confidence level, `=CONFIDENCE.NORM(0.1,15,40)` returns approximately 3.90. Adding and subtracting this from $\bar{x}$ gives the confidence interval (102.4, 110.2).
 
### Desmos
You can use Desmos the same way as in [18.1](18_1_CriticalValues.md) to find the critical value, then calculate the margin of error and the confidence interval boundaries by hand using the equations from this lesson.
 
Alternatively, you can let Desmos do the arithmetic for you:
* Define your values as variables, for example: `xbar = 106.3`, `sigma = 15`, `n = 40`, `z_c = 1.645`
* Type `E = z_c * sigma / sqrt(n)` to calculate the margin of error
* Type `xbar + E` and `xbar - E` to find the upper and lower boundaries of the confidence interval
Desmos will calculate and display each of these values as soon as they are typed in.