<head>
<title>24.4 Hypothesis Test for the Mean Difference</title>
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

# Lesson 24.4 Hypothesis Test for the Mean Difference
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.1 Paired data (page 209)

## Lesson
We now combine Lessons 24.1–24.3 into the same five-step hypothesis test we used in Lesson 20.5 — applied to $d$ instead of $x$, with a null value of 0. If this feels like review, that's the point: **a paired test is just a one-sample t-test on the differences.**

### The Five Steps

**Step 1 — Verify the Conditions**
* Is the sample of pairs random?
* Is $n \ge 30$, or are the differences approximately normally distributed?

**Step 2 — State the Hypotheses**

$$H_0: \mu_d = 0 \qquad H_A: \mu_d > 0 \text{ or } \mu_d < 0 \text{ or } \mu_d \ne 0$$

**Step 3 — Compute the Test Statistic**

$$t = \frac{\bar{d} - 0}{s_d/\sqrt{n}} \qquad\qquad df = n-1$$

**Step 4 — Find the Critical Value and/or P-Value**

| Test Type | Critical value | P-value |
|---|---|---|
| Right-tailed | $t_c$ | $P(T > t)$ |
| Left-tailed | $-t_c$ | $P(T < t)$ |
| Two-tailed | $\pm t_c$ | $2 \times P(T > \vert t \vert)$ |

**Step 5 — Make a Decision and Write a Conclusion**
* Reject $H_0$ if the test statistic falls in the critical region, or if $p\text{-value} \le \alpha$.
* Write a plain-language conclusion in terms of the two original (paired) variables.

---

### Example

> A clinic wants to know whether a new medication lowers systolic blood pressure. Blood pressure is measured for 10 patients before starting the medication, and again after 4 weeks. Test at the 5% significance level.

From Lessons 24.1–24.2: $\bar{d} = 6.5$, $s_d \approx 2.677$, $n = 10$ ($d = \text{Before} - \text{After}$).

**Step 1 — Verify the Conditions**
* Random? **Yes**
* $n = 10 < 30$, but the 10 differences are reasonably symmetric with no extreme outliers, so we treat the normality condition as satisfied.

**Step 2 — Hypotheses**

$$H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d > 0 \quad \text{(right-tailed)}$$

**Step 3 — Test Statistic**

$$SE = \frac{2.677}{\sqrt{10}} \approx 0.8465$$

$$t = \frac{6.5 - 0}{0.8465} \approx 7.678 \qquad\qquad df = 9$$

**Step 4 — Critical Value and P-Value**

* Critical value (right-tailed, $\alpha = 0.05$, $df = 9$): $t_c \approx 1.833$
* P-value: $p < 0.0001$

**Step 5 — Decision and Conclusion**

* $t = 7.678 > t_c = 1.833$ → **Reject $H_0$**
* $p < 0.0001 \le \alpha = 0.05$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the medication lowers systolic blood pressure. This matches the 90% confidence interval from Lesson 24.3, which was entirely above 0.

## Practice
1. A researcher tests whether caffeine improves (lowers) reaction time, using $d = \text{Before} - \text{After}$ ($\bar{d} = 17.2$, $s_d \approx 8.928$, $n = 5$). Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/24_4_Solution1.md)
2. An instructor wants to know if a review session improves (raises) exam scores, using $d = \text{Posttest} - \text{Pretest}$ ($\bar{d} \approx 3.833$, $s_d \approx 2.787$, $n = 6$). Conduct a full hypothesis test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/24_4_Solution2.md)
3. A nutritionist wants to know if a 6-week diet program changes participants' weight, using $d = \text{Before} - \text{After}$ ($\bar{d} = 6.6$, $s_d \approx 1.517$, $n = 5$). Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/24_4_Solution3.md)

## Technology
### TI-83/84
* Press `STAT` → `Edit...`
* Enter the "Before" values in `L1` and the "After" values in `L2`
* Highlight the `L3` header, type `L1-L2`, and press `Enter` to fill `L3` with the differences
* Press `STAT` → `[TESTS]` → `2:T-Test...`
* Choose `Data`, set `List` to `L3` and `Freq` to `1`, and set $\mu_0 = 0$
* Choose the direction of $H_A$
* Select `Calculate`

The calculator returns the test statistic (`t`), the p-value, and the degrees of freedom (`df`). If you only have summary statistics ($\bar{d}$, $s_d$, $n$), choose `Stats` instead of `Data` and enter them directly.

### Excel
1. Build a column of differences from the raw data (or start from your known $\bar{d}$ and $s_d$)
2. Find the standard error: `=sd/SQRT(n)`
3. Find the test statistic: `=dbar/SE`
4. Find the p-value using `T.DIST`:
    * Right-tailed: `=1-T.DIST(t,df,TRUE)`
    * Left-tailed: `=T.DIST(t,df,TRUE)`
    * Two-tailed: `=T.DIST.2T(ABS(t),df)`

If you have the raw paired data in two columns, Excel's `=T.TEST(array1,array2,tails,1)` function computes the p-value directly, where `tails` is `1` or `2` and the final `1` tells Excel to use the **paired** version of the test.

### Desmos
In [Desmos](www.desmos.com/calculator), type the test statistic formula directly:

$$t = \frac{6.5}{2.677/\sqrt{10}}$$

Replace the values with those from your own problem, and compare the result to the critical value found from the TI-84 or a t-table (using $df = n-1$) to make your decision.
