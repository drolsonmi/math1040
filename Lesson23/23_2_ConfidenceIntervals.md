<head>
<title>23.2 Confidence Intervals for 2 Independent Samples</title>
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

# Lesson 23.2 Confidence Intervals for 2 Independent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.2.2 Confidence interval for a difference of proportions (pages 244-246)

## Lesson
Just as with means, we can build a confidence interval for the **difference between two proportions**, $p_1 - p_2$.

### The Point Estimate
$$\hat{p}_1 - \hat{p}_2$$

### The Standard Error
Unlike the hypothesis test, a confidence interval does **not** assume $H_0$ is true — so here we do *not* pool the two proportions. Instead, we use each sample's own proportion:

$$SE = \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$$

### The Confidence Interval
$$(\hat{p}_1 - \hat{p}_2) \pm z_c \cdot SE$$

Since proportions always use the z-distribution, the critical value comes from the same standard normal table we've used since Lesson 19.

> __Note:__ Just as in Lesson 22.3, use a confidence level of $1-2\alpha$ if you're building the interval to match a one-tailed test, or $1-\alpha$ for a two-tailed test.

### Interpreting the Interval
* Entirely **above 0**: evidence that $p_1 > p_2$
* Entirely **below 0**: evidence that $p_1 < p_2$
* **Contains 0**: not enough evidence that the two proportions are different

### Example

> A wellness organization wants to know if the proportion of adults who exercise regularly is different between City A and City B. A random sample of 250 adults in City A found that 140 exercise regularly. An independent random sample of 230 adults in City B found that 110 exercise regularly. Build a 95% confidence interval for $p_1 - p_2$.

From Lesson 23.1:
* $\hat{p}_1 = 0.56$, $n_1 = 250$
* $\hat{p}_2 \approx 0.478$, $n_2 = 230$
* Conditions verified ✓

**Point Estimate:**

$$\hat{p}_1 - \hat{p}_2 = 0.56 - 0.478 = 0.082$$

**Standard Error:**

$$SE = \sqrt{\frac{0.56(0.44)}{250}+\frac{0.478(0.522)}{230}} = \sqrt{0.000986+0.001085} = \sqrt{0.002070} \approx 0.0455$$

**Critical Value** (95% confidence, two-tailed): $z_c = 1.960$

**Confidence Interval:**

$$0.082 \pm 1.960(0.0455) = 0.082 \pm 0.0892$$

$$(-0.007, \ 0.171)$$

**Interpretation:** We are 95% confident that the true difference in exercise rates between City A and City B ($p_1 - p_2$) is between -0.007 and 0.171 (-0.7 and 17.1 percentage points). Since the interval **contains 0**, we don't have enough evidence to say the two cities have different exercise rates.

## Practice
1. A marketing team wants to know if customer satisfaction differs between two products. A random sample of 180 Product A customers found 126 satisfied. An independent random sample of 165 Product B customers found 90 satisfied. Build a 95% confidence interval for $p_1 - p_2$.
    * [After solving on your own, see solution here](./Solutions/23_2_Solution1.md)
2. A public health department wants to know if a new smoking cessation program has a higher success rate than the standard program. A random sample of 140 participants in the new program found that 42 successfully quit smoking. An independent random sample of 150 participants in the standard program found that 27 successfully quit. Build a 98% confidence interval for $p_1 - p_2$.
    * [After solving on your own, see solution here](./Solutions/23_2_Solution2.md)
3. A quality control manager wants to know if Machine A has a lower defect rate than Machine B. A random sample of 200 items from Machine A found 14 defective. An independent random sample of 220 items from Machine B found 24 defective. Build a 90% confidence interval for $p_1 - p_2$.
    * [After solving on your own, see solution here](./Solutions/23_2_Solution3.md)

## Technology
### TI-83/84
* Press `STAT`
* Select the `TESTS` menu
* Select `B:2-PropZInt...`
* Enter $x_1$, $n_1$, $x_2$, $n_2$, and the confidence level (C-Level)
* Select `Calculate`

The calculator returns the confidence interval bounds, along with $\hat{p}_1$ and $\hat{p}_2$.

### Excel
Just as with means, build the interval from its pieces — no pooling this time.

1. Find each sample proportion: `=x1/n1` and `=x2/n2`
2. Find the point estimate: `=phat1-phat2`
3. Find the standard error: `=SQRT(phat1*(1-phat1)/n1+phat2*(1-phat2)/n2)`
4. Find the critical value with `NORM.S.INV`, entering the area to the left of $z_c$: for a 95% CI, type `=NORM.S.INV(0.975)`
5. Find the margin of error: `=zc*SE`
6. Find the boundaries: `=estimate-E` and `=estimate+E`

For example, with $\hat p_1$ in B1, $\hat p_2$ in B2, $n_1$ in B3, and $n_2$ in B4, the standard error formula would be `=SQRT(B1*(1-B1)/B3+B2*(1-B2)/B4)`.

### Desmos
In [Desmos](www.desmos.com/calculator), type the point estimate and standard error directly:

$$\text{Estimate} = 0.56 - 0.478 \qquad\qquad SE = \sqrt{\frac{0.56(0.44)}{250}+\frac{0.478(0.522)}{230}}$$

Then compute the boundaries using the critical value found with the inverse-normal method from Lesson 18.1:

$$\text{Lower} = 0.082 - 1.96\sqrt{\frac{0.56(0.44)}{250}+\frac{0.478(0.522)}{230}} \qquad\qquad \text{Upper} = 0.082 + 1.96\sqrt{\frac{0.56(0.44)}{250}+\frac{0.478(0.522)}{230}}$$

Replace the values with those from your own problem.
