<head>
<title>22.4 Hypothesis Test of 2 Independent Samples</title>
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

# Lesson 22.4 Hypothesis Test of 2 Independent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.4 Hypothesis test for a difference of means (pages 215-217)

## Lesson
We now combine Lessons 22.1–22.3 into the same five-step hypothesis test we used in Lesson 20, applied to two independent means.

### The Five Steps

**Step 1 — Verify the Conditions**
* Are both samples random?
* Are the two samples independent of each other?
* Is each sample large enough ($n \ge 30$, or the population is normal)?

**Step 2 — State the Hypotheses**

$$H_0: \mu_1 = \mu_2 \qquad H_A: \mu_1 > \mu_2 \text{ or } \mu_1 < \mu_2 \text{ or } \mu_1 \ne \mu_2$$

**Step 3 — Compute the Test Statistic**

$$t = \frac{(\bar{x}_1 - \bar{x}_2) - 0}{\sqrt{\dfrac{s_1^2}{n_1}+\dfrac{s_2^2}{n_2}}}$$

The "$-0$" is there to remind you that we're comparing the observed difference to a null difference of exactly 0 — you'll rarely need to write it out, since subtracting 0 doesn't change anything.

**Step 4 — Find the Critical Value and/or P-Value**

| Test Type    | Critical value | P-value                         |
| :----------- | :------------: | :-----------------------------: |
| Right-tailed | $t_c$          | $P(T > t)$                      |
| Left-tailed  | $-t_c$         | $P(T < t)$                      |
| Two-tailed   | $\pm t_c$      | $2 \times P(T > \vert t \vert)$ |

As with the confidence interval, technology finds the degrees of freedom for us.

**Step 5 — Make a Decision and Write a Conclusion**
* Reject $H_0$ if the test statistic falls in the critical region, or if $p\text{-value} \le \alpha$.
* Write a plain-language conclusion in terms of the original two groups.

---

### Example

> A city wants to know whether the average customer wait time is different between its two coffee shop locations. A random sample of 32 customers at Location A had an average wait time of 4.8 minutes with a standard deviation of 1.1 minutes. An independent random sample of 35 customers at Location B had an average wait time of 4.3 minutes with a standard deviation of 0.9 minutes. Test at the 5% significance level.

**Step 1 — Verify the Conditions**
* Random? **Yes**
* Independent? **Yes** — different customers at two different locations
* Large enough? $n_1 = 32 \ge 30$ ✓ and $n_2 = 35 \ge 30$ ✓

**Step 2 — Hypotheses**

$$H_0: \mu_1 = \mu_2 \qquad\qquad H_A: \mu_1 \ne \mu_2 \quad \text{(two-tailed)}$$

**Step 3 — Test Statistic**

$$SE = \sqrt{\frac{1.1^2}{32}+\frac{0.9^2}{35}} \approx 0.2469$$

$$t = \frac{4.8-4.3}{0.2469} = \frac{0.5}{0.2469} \approx 2.025$$

**Step 4 — Critical Value and P-Value**

* Critical value (two-tailed, $\alpha = 0.05$, $df \approx 63.7$): $t_c \approx \pm 1.998$
* P-value: $p \approx 0.047$

**Step 5 — Decision and Conclusion**

* $|t| = 2.025 > t_c = 1.998$ → **Reject $H_0$**
* $p \approx 0.047 \le \alpha = 0.05$ → **Reject $H_0$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the average customer wait time is different between the two coffee shop locations. This matches the 95% confidence interval we found in Lesson 22.3, which barely excluded 0.

## Practice
1. An education researcher wants to know if there is a difference in average test scores between School A and School B. A random sample of 40 students at School A had an average score of 78.4 with a standard deviation of 8.2. An independent random sample of 38 students at School B had an average score of 74.9 with a standard deviation of 7.5. Conduct a full hypothesis test at the 5% significance level (use $df \approx 75.7$).
    * [After solving on your own, see solution here](./Solutions/22_4_Solution1.md)
2. A fitness researcher wants to know if Program X leads to greater average weight loss than Program Y. A random sample of 25 participants using Program X lost an average of 12.3 lbs with a standard deviation of 3.1 lbs. An independent random sample of 28 participants using Program Y lost an average of 9.8 lbs with a standard deviation of 2.8 lbs. Conduct a full hypothesis test at the 1% significance level (use $df \approx 49.8$).
    * [After solving on your own, see solution here](./Solutions/22_4_Solution2.md)
3. A transit planner wants to know if Bus Route 1 has a shorter average travel time than Bus Route 2. A random sample of 30 trips on Route 1 averaged 22.5 minutes with a standard deviation of 4.0 minutes. An independent random sample of 32 trips on Route 2 averaged 25.1 minutes with a standard deviation of 4.6 minutes. Conduct a full hypothesis test at the 5% significance level (use $df \approx 59.5$).
    * [After solving on your own, see solution here](./Solutions/22_4_Solution3.md)

## Technology
### TI-83/84
* Press `STAT`
* Select the `TESTS` menu
* Select `4:2-SampTTest...`
* Choose `Stats`, then enter $\bar{x}_1$, $s_1$, $n_1$, $\bar{x}_2$, $s_2$, $n_2$
* Choose the direction of $H_A$ ($\ne$, $<$, or $>$)
* For `Pooled`, select `No`
* Select `Calculate`

The calculator returns the test statistic (`t`), the p-value, and the degrees of freedom (`df`) it used.

### Excel
Build the test statistic and p-value from their pieces, using the same standard error as Lesson 22.3.

__Test Statistic:__
* `=(xbar1-xbar2)/SQRT(s1^2/n1+s2^2/n2)` (e.g., `=(B1-B2)/SQRT(B3^2/B5+B4^2/B6)`)

__P-value:__ use `T.DIST` for a left-tailed p-value, `1-T.DIST` for right-tailed, or `T.DIST.2T` for two-tailed, plugging in your test statistic and the degrees of freedom found on the TI-84 or Desmos.
* Right-tailed: `=1-T.DIST(t,df,TRUE)`
* Left-tailed: `=T.DIST(t,df,TRUE)`
* Two-tailed: `=T.DIST.2T(ABS(t),df)`

If you have the raw data (not just summary statistics) for both samples, Excel's `=T.TEST(array1,array2,tails,3)` function will compute the p-value for you directly, where `tails` is `1` for a one-tailed test or `2` for a two-tailed test, and `3` tells Excel to use the unequal-variance (Welch) version.

### Desmos
In [Desmos](www.desmos.com/calculator), type the test statistic formula directly:

$$t = \frac{4.8-4.3}{\sqrt{\dfrac{1.1^2}{32}+\dfrac{0.9^2}{35}}}$$

Replace the values with those from your own problem, and compare the result to the critical value you found (from the TI-84 or a t-table, using the given degrees of freedom) to make your decision.
