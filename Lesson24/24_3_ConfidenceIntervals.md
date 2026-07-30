<head>
<title>24.3 Confidence Interval for the Mean Difference</title>
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

# Lesson 24.3 Confidence Interval for the Mean Difference
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.1 Paired data (page 209)

## Lesson
Since a paired-difference problem is really a one-sample problem in disguise, building a confidence interval for $\mu_d$ is exactly the t-interval from Lesson 18 — just applied to $d$.

#### The Confidence Interval

$$\bar{d} \pm t_c \cdot \frac{s_d}{\sqrt{n}}$$

The critical value $t_c$ comes from the t-distribution with $df = n - 1$, exactly as in Lesson 18.5, where $n$ is the number of *pairs*.

> __Note:__ As in Lessons 22.3 and 23.2, use a confidence level of $1-2\alpha$ if the interval is meant to correspond to a one-tailed test, or $1-\alpha$ for a two-tailed test.

#### Interpreting the Interval
* Entirely **above 0**: evidence that $\mu_d > 0$
* Entirely **below 0**: evidence that $\mu_d < 0$
* **Contains 0**: not enough evidence that there's a real difference

Remember that the sign of $\bar{d}$ (and therefore the interval) depends entirely on the order of subtraction you chose in Lesson 24.1 — always interpret the interval in terms of the original variables, not just the number.

#### Example

> A clinic wants to know whether a new medication lowers systolic blood pressure. Blood pressure is measured for 10 patients before starting the medication, and again after 4 weeks. Build a 90% confidence interval for the mean difference.

From Lessons 24.1–24.2: $\bar{d} = 6.5$, $s_d \approx 2.677$, $n = 10$ ($d = \text{Before} - \text{After}$), conditions verified ✓.

We use a 90% confidence level here since this interval is meant to correspond to the one-tailed test ($\alpha = 0.05$) from Lesson 24.2: $1-2(0.05) = 0.90$.

**Standard Error:**

$$SE = \frac{s_d}{\sqrt{n}} = \frac{2.677}{\sqrt{10}} \approx 0.8465$$

**Critical Value** ($df = 9$, 90% confidence): $t_c \approx 1.833$

**Confidence Interval:**

$$6.5 \pm 1.833(0.8465) = 6.5 \pm 1.552$$

$$(4.948, \ 8.052)$$

**Interpretation:** We are 90% confident that the true mean reduction in systolic blood pressure ($\mu_d$) after taking the medication is between 4.948 and 8.052 points. Since the entire interval is above 0, there is evidence that the medication lowers systolic blood pressure.

## Practice
1. A researcher tests whether caffeine improves (lowers) reaction time, using $d = \text{Before} - \text{After}$ ($\bar{d} = 17.2$, $s_d \approx 8.928$, $n = 5$). Build a 90% confidence interval for $\mu_d$.
    * [After solving on your own, see solution here](./Solutions/24_3_Solution1.md)
2. An instructor wants to know if a review session improves (raises) exam scores, using $d = \text{Posttest} - \text{Pretest}$ ($\bar{d} \approx 3.833$, $s_d \approx 2.787$, $n = 6$). Build a 98% confidence interval for $\mu_d$.
    * [After solving on your own, see solution here](./Solutions/24_3_Solution2.md)
3. A nutritionist wants to know if a 6-week diet program changes participants' weight, using $d = \text{Before} - \text{After}$ ($\bar{d} = 6.6$, $s_d \approx 1.517$, $n = 5$). Build a 95% confidence interval for $\mu_d$.
    * [After solving on your own, see solution here](./Solutions/24_3_Solution3.md)

## Technology
### TI-83/84
The easiest approach is to enter both lists of raw data and let the calculator build the differences for you.
* Press `STAT` → `Edit...`
* Enter the "Before" values in `L1` and the "After" values in `L2`
* Move the cursor to highlight the `L3` header, then type `L1-L2` and press `Enter` — this fills `L3` with the differences
* Press `STAT` → `[TESTS]` → `8:TInterval...`
* Choose `Data`, set `List` to `L3`, and `Freq` to `1`
* Enter the confidence level (C-Level)
* Select `Calculate`

If you only have the summary statistics ($\bar{d}$, $s_d$, $n$) rather than the raw data, choose `Stats` instead of `Data` and enter them directly.

### Excel
1. Enter the "Before" and "After" values in two columns, then create a third column of differences (e.g., `=A2-B2`, filled down)
2. Find $\bar{d}$: `=AVERAGE(range)`
3. Find $s_d$: `=STDEV.S(range)`
4. Find the standard error: `=sd/SQRT(n)` (e.g., `=B1/SQRT(B2)`)
5. Find the critical value: `=T.INV.2T(alpha,df)` — for a 90% CI, $\alpha = 0.10$, so type `=T.INV.2T(0.10,9)`
6. Find the margin of error: `=tc*SE`
7. Find the boundaries: `=dbar-E` and `=dbar+E`

### Desmos
In [Desmos](www.desmos.com/calculator), type the standard error directly, then compute the boundaries using a critical value found from the TI-84 or a t-table:

$$SE = \frac{2.677}{\sqrt{10}}$$

$$\text{Lower} = 6.5 - 1.833\left(\frac{2.677}{\sqrt{10}}\right) \qquad\qquad \text{Upper} = 6.5 + 1.833\left(\frac{2.677}{\sqrt{10}}\right)$$

Replace the values with those from your own problem.
