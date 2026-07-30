<head>
<title>22.3 Confidence Intervals for 2 Independent Samples</title>
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

# Lesson 22.3 Confidence Intervals for 2 Independent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.3 Confidence interval for a difference of means (pages 212-214)

## Lesson
Just as we built a confidence interval for a single mean, we can build one for the **difference between two means**, $\mu_1 - \mu_2$. The structure is exactly the same as before: a point estimate, plus or minus a margin of error.

### The Point Estimate
Our best estimate of $\mu_1 - \mu_2$ is simply the difference between the two sample means:

$$\bar{x}_1 - \bar{x}_2$$

### The Standard Error
Since the two samples are independent, we combine their individual variabilities like this:

$$SE = \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$$

### The Confidence Interval
$$(\bar{x}_1 - \bar{x}_2) \pm t_c \cdot SE$$

Just like the one-sample t-interval, the critical value $t_c$ comes from a t-distribution. The degrees of freedom for two independent samples is more complicated than $n-1$, so we let technology calculate it for us (this is often called the Welch approximation).

> __Note:__ If a one-tailed hypothesis test is what you're ultimately after, use a confidence level of $1-2\alpha$ to build a two-sided interval that corresponds to that one-tailed test, just as we did in Lesson 20. For a two-tailed test, use $1-\alpha$.

### Interpreting the Interval
* If the interval is entirely **above 0**, we have evidence that $\mu_1 > \mu_2$
* If the interval is entirely **below 0**, we have evidence that $\mu_1 < \mu_2$
* If the interval **contains 0**, we don't have enough evidence to say the means are different at all

### Example

> A city wants to know whether the average customer wait time is different between its two coffee shop locations. A random sample of 32 customers at Location A had an average wait time of 4.8 minutes with a standard deviation of 1.1 minutes. An independent random sample of 35 customers at Location B had an average wait time of 4.3 minutes with a standard deviation of 0.9 minutes. Build a 95% confidence interval for $\mu_1 - \mu_2$.

From Lesson 22.2:
* $n_1 = 32$, $\bar{x}_1 = 4.8$, $s_1 = 1.1$
* $n_2 = 35$, $\bar{x}_2 = 4.3$, $s_2 = 0.9$
* Conditions verified ✓

**Point Estimate:**

$$\bar{x}_1 - \bar{x}_2 = 4.8 - 4.3 = 0.5$$

**Standard Error:**

$$SE = \sqrt{\frac{1.1^2}{32} + \frac{0.9^2}{35}} = \sqrt{0.03781 + 0.02314} = \sqrt{0.06096} \approx 0.2469$$

**Critical Value** (technology gives $df \approx 63.7$, 95% confidence): $t_c \approx 1.998$

**Confidence Interval:**

$$0.5 \pm 1.998(0.2469) = 0.5 \pm 0.493$$

$$(0.007, \ 0.993)$$

**Interpretation:** We are 95% confident that the true difference in average wait time between Location A and Location B ($\mu_1 - \mu_2$) is between 0.007 and 0.993 minutes. Since the entire interval is above 0 (barely!), there is evidence that Location A's average wait time is longer than Location B's.

## Practice
1. An education researcher wants to know if there is a difference in average test scores between School A and School B. A random sample of 40 students at School A had an average score of 78.4 with a standard deviation of 8.2. An independent random sample of 38 students at School B had an average score of 74.9 with a standard deviation of 7.5. Build a 95% confidence interval for $\mu_1 - \mu_2$ (use $df \approx 75.7$).
    * [After solving on your own, see solution here](./Solutions/22_3_Solution1.md)
2. A fitness researcher wants to know if Program X leads to greater average weight loss than Program Y. A random sample of 25 participants using Program X lost an average of 12.3 lbs with a standard deviation of 3.1 lbs. An independent random sample of 28 participants using Program Y lost an average of 9.8 lbs with a standard deviation of 2.8 lbs. Build a 98% confidence interval for $\mu_1 - \mu_2$ (use $df \approx 49.8$).
    * [After solving on your own, see solution here](./Solutions/22_3_Solution2.md)
3. A transit planner wants to know if Bus Route 1 has a shorter average travel time than Bus Route 2. A random sample of 30 trips on Route 1 averaged 22.5 minutes with a standard deviation of 4.0 minutes. An independent random sample of 32 trips on Route 2 averaged 25.1 minutes with a standard deviation of 4.6 minutes. Build a 90% confidence interval for $\mu_1 - \mu_2$ (use $df \approx 59.5$).
    * [After solving on your own, see solution here](./Solutions/22_3_Solution3.md)

## Technology
### TI-83/84
* Press `STAT`
* Select the `TESTS` menu
* Select `0:2-SampTInt...`
* Choose `Stats`, then enter $\bar{x}_1$, $s_1$, $n_1$, $\bar{x}_2$, $s_2$, $n_2$, and the confidence level (C-Level)
* For `Pooled`, select `No` (we don't assume the two population variances are equal)
* Select `Calculate`

The calculator returns the confidence interval bounds, along with the degrees of freedom (`df`) it used.

### Excel
Excel does not have a single 2-sample confidence interval function, so we build it from its pieces.

1. Find the point estimate: `=xbar1-xbar2` (e.g., `=B1-B2`)
2. Find the standard error: `=SQRT(s1^2/n1+s2^2/n2)` (e.g., `=SQRT(B3^2/B5+B4^2/B6)`)
3. Find the critical value using `T.INV.2T`, which returns the two-tailed critical value directly:
    * `=T.INV.2T(alpha, df)` — for a 95% CI, $\alpha = 0.05$, so type `=T.INV.2T(0.05,63.7)`
4. Find the margin of error: `=tc*SE` (e.g., `=B7*B8`)
5. Find the boundaries: `=estimate-E` and `=estimate+E`

Excel can also calculate the (Welch) degrees of freedom directly with `=T.TEST(range1,range2,2,3)` paired with raw data, but when you only have summary statistics ($\bar{x}$, $s$, $n$), the TI-84 or Desmos is often faster for finding $df$.

### Desmos
In [Desmos](www.desmos.com/calculator), type the point estimate and standard error directly:

$$\text{Estimate} = 4.8 - 4.3 \qquad\qquad SE = \sqrt{\frac{1.1^2}{32}+\frac{0.9^2}{35}}$$

Once you have a critical value (from the TI-84 or a t-table using the given degrees of freedom), you can compute the boundaries directly:

$$\text{Lower} = 0.5 - 1.998\sqrt{\frac{1.1^2}{32}+\frac{0.9^2}{35}} \qquad\qquad \text{Upper} = 0.5 + 1.998\sqrt{\frac{1.1^2}{32}+\frac{0.9^2}{35}}$$

Replace the values with those from your own problem.
