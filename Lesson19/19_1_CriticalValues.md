<head>
<title>19.1 Critical Values for Proportion Confidence Intervals</title>
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

# Lesson 19.1 Critical Value and Margin of Error for a Proportion
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.1.1 Confidence intervals for a proportion (pages 218–222)

## Lesson
In Lesson 18, we found confidence intervals for quantitative variables — problems that involved a mean. Now we turn to __categorical variables__, where we are interested in a __proportion__. Here is the problem we will work on through this lesson:

> A local college wants to estimate the true proportion of its students who work a part-time job. A random sample of 200 students is taken, and 130 of them report working part-time. What is the true proportion of students at this college who work part-time?

We can't find the exact value for the true proportion without surveying every student. Instead, we will construct a __confidence interval__ — a range of values in which the true proportion is likely to fall.

Before we can do that, we need to verify that the Central Limit Theorem applies, find our critical value, and compute the margin of error.

### Setting Up: The Sample Proportion

The first thing we need is the __sample proportion__ ($\hat{p}$, read "p-hat"), which is the proportion observed in our sample.

$$\hat{p} = \frac{x}{n}$$

where $$x$$ is the number of individuals in the sample with the characteristic of interest, and $$n$$ is the sample size. For our scenario,

$$\hat{p} = \frac{130}{200} = 0.65$$

It is also useful to define $\hat{q}$, which is the proportion of the sample *without* the characteristic:

$$\hat{q} = 1 - \hat{p} = 1 - 0.65 = 0.35$$

### Conditions for the Central Limit Theorem

Just as we needed the sample to be large enough when working with means, we need to verify two conditions before constructing a confidence interval for a proportion:

* __The sample must be random__, and
* __The sample must be large enough__. For proportions, we require both $n\hat{p} \ge 10$ __and__ $n\hat{q} \ge 10$.

The second condition ensures that there are enough observed "successes" and "failures" for the normal approximation to be reliable.

For our scenario:
* The sample is stated to be random — *this is satisfied*
* $n\hat{p} = 200(0.65) = 130 \ge 10$ — *this is satisfied*
* $n\hat{q} = 200(0.35) = 70 \ge 10$ — *this is satisfied*

Since both conditions are satisfied, the Central Limit Theorem applies and we can proceed.

### Critical Values

The critical value for a proportion confidence interval is the same z-score we used in [Lesson 18.1](../Lesson18/18_1_CriticalValues.md). The three most common confidence levels and their critical values are repeated here:

| Confidence Level | Critical Value |
| :--------------: | :------------: |
|     90%          |  $\pm 1.645$   |
|     95%          |  $\pm 1.96$    |
|     99%          |  $\pm 2.58$    |

We will use a 95% confidence level for our scenario, so $z_c = \pm 1.96$.

### Margin of Error

The __margin of error__ for a proportion is:

$$E = z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} = z_c\sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$$

This formula is analogous to the margin of error for a mean ($E = z_c \cdot \sigma/\sqrt{n}$) — the critical value multiplied by the standard error. The key difference is that the error is now computed from $\hat{p}$ instead of a known population standard deviation.

For our scenario at the 95% confidence level,

$$\begin{align*}
E &= z_c\sqrt{\frac{\hat{p}\hat{q}}{n}} = z_c\sqrt{\frac{\hat{p}(1-\hat{p})}{n}} \\
  &= 1.96\sqrt{\frac{(0.65)(0.35)}{200}} \\
  &= 1.96 \times 0.03373 \\
  &\approx \mathbf{0.066}
\end{align*}$$

The margin of error is approximately **0.066**, or **6.6 percentage points**. We will use this in the next lesson to construct the full confidence interval.

## Practice
1. A poll asks whether registered voters plan to vote in the upcoming election. In a random sample of 150 voters, 96 say they plan to vote. Find the margin of error at the 90% confidence level.
    * [After solving on your own, see solution here](Solutions/19_1_Solution1.md)
2. A random sample of 400 households in a city finds that 112 own a pet. Find the margin of error at the 95% confidence level.
    * [After solving on your own, see solution here](Solutions/19_1_Solution2.md)
3. A health survey of 250 randomly selected adults finds that 85 report exercising at least 3 times per week. Find the margin of error at the 99% confidence level.
    * [After solving on your own, see solution here](Solutions/19_1_Solution3.md)

## Technology
### TI-83/84
You can find the margin of error for a proportion by calculating the confidence interval and reading off the bounds. On the TI-83/84:
* Press `STAT`
* Select the `TESTS` menu
* Select `A:1-PropZInt...`
* Enter $$x$$ (number of successes), $$n$$ (sample size), and the confidence level (C-Level)
* Select "Calculate"

The calculator will return the lower and upper bounds of the confidence interval. The margin of error is half the width of the interval:

$$E = \frac{\text{Upper Bound} - \text{Lower Bound}}{2}$$

### Desmos
To find critical values in [Desmos](www.desmos.com/calculator), follow the same steps described in Lesson 18.1 — the critical values come from the same standard normal distribution regardless of whether you are working with means or proportions.

To compute the margin of error directly, you can type the formula into Desmos:

$$E = 1.96\sqrt{\frac{0.65 \times 0.35}{200}}$$

Replace the values of $z_c$, $\hat{p}$, $\hat{q}$, and $$n$$ with those from your problem.