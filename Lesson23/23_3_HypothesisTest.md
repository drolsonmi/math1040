<head>
<title>23.3 Hypothesis Test of 2 Independent Samples</title>
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

# Lesson 23.3 Hypothesis Test of 2 Independent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.2.3 Hypothesis test for a difference of proportions (pages 246-248)

## Lesson
We now combine Lessons 23.1–23.2 into the same five-step hypothesis test we've used throughout this course, applied to two independent proportions.

### The Five Steps

**Step 1 — Verify the Conditions**
* Are both samples random?
* Are the two samples independent of each other?
* Does the success-failure condition hold for both samples, using the **pooled** proportion $\bar{p}$?

**Step 2 — State the Hypotheses**

$$H_0: p_1 = p_2 \qquad H_A: p_1 > p_2 \text{ or } p_1 < p_2 \text{ or } p_1 \ne p_2$$

**Step 3 — Compute the Test Statistic**

Unlike the confidence interval, the hypothesis test *does* assume $H_0$ is true, so we use the pooled proportion in the standard error:

$$z = \frac{\hat{p}_1 - \hat{p}_2}{\sqrt{\bar{p}(1-\bar{p})\left(\dfrac{1}{n_1}+\dfrac{1}{n_2}\right)}}$$

**Step 4 — Find the Critical Value and/or P-Value**

| Test Type    | Critical value | P-value                         |
| :----------- | :------------: | :-----------------------------: |
| Right-tailed | $z_c$          | $P(Z > z)$                      |
| Left-tailed  | $-z_c$         | $P(Z < z)$                      |
| Two-tailed   | $\pm z_c$      | $2 \times P(Z > \vert z \vert)$ |

**Step 5 — Make a Decision and Write a Conclusion**
* Reject $H_0$ if the test statistic falls in the critical region, or if $p\text{-value} \le \alpha$.
* Write a plain-language conclusion in terms of the original two groups.

---

### Example

> A wellness organization wants to know if the proportion of adults who exercise regularly is different between City A and City B. A random sample of 250 adults in City A found that 140 exercise regularly. An independent random sample of 230 adults in City B found that 110 exercise regularly. Test at the 5% significance level.

**Step 1 — Verify the Conditions**
* Random? **Yes**
* Independent? **Yes** — different adults in two different cities
* Pooled proportion: $\bar{p} = \dfrac{140+110}{250+230} \approx 0.521$; all four success-failure checks pass (see Lesson 23.1) ✓

**Step 2 — Hypotheses**

$$H_0: p_1 = p_2 \qquad\qquad H_A: p_1 \ne p_2 \quad \text{(two-tailed)}$$

**Step 3 — Test Statistic**

$$\hat{p}_1 = 0.56 \qquad \hat{p}_2 \approx 0.478$$

$$SE = \sqrt{0.521(0.479)\left(\frac{1}{250}+\frac{1}{230}\right)} \approx 0.04565$$

$$z = \frac{0.56-0.478}{0.04565} = \frac{0.082}{0.04565} \approx 1.790$$

**Step 4 — Critical Value and P-Value**

* Critical value (two-tailed, $\alpha = 0.05$): $z_c = \pm 1.960$
* P-value: $p = 2 \times P(Z > 1.790) \approx 2 \times 0.0367 = 0.0734$

**Step 5 — Decision and Conclusion**

* $|z| = 1.790 < z_c = 1.960$ → **Fail to reject $H_0$**
* $p \approx 0.0734 > \alpha = 0.05$ → **Fail to reject $H_0$**

**Conclusion:** There is not enough evidence at the 5% significance level to conclude that the proportion of adults who exercise regularly is different between City A and City B. This matches the confidence interval we found in Lesson 23.2, which contained 0.

## Practice
1. A marketing team wants to know if customer satisfaction differs between two products. A random sample of 180 Product A customers found 126 satisfied. An independent random sample of 165 Product B customers found 90 satisfied. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/23_3_Solution1.md)
2. A public health department wants to know if a new smoking cessation program has a higher success rate than the standard program. A random sample of 140 participants in the new program found that 42 successfully quit smoking. An independent random sample of 150 participants in the standard program found that 27 successfully quit. Conduct a full hypothesis test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/23_3_Solution2.md)
3. A quality control manager wants to know if Machine A has a lower defect rate than Machine B. A random sample of 200 items from Machine A found 14 defective. An independent random sample of 220 items from Machine B found 24 defective. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/23_3_Solution3.md)

## Technology
### TI-83/84
* Press `STAT`
* Select the `TESTS` menu
* Select `6:2-PropZTest...`
* Enter $x_1$, $n_1$, $x_2$, $n_2$
* Choose the direction of $H_A$ ($\ne$, $<$, or $>$)
* Select `Calculate`

The calculator returns the pooled test statistic (`z`), the p-value, $\hat{p}_1$, $\hat{p}_2$, and the pooled proportion $\bar{p}$.

### Excel
Build the test statistic and p-value from their pieces, using the pooled proportion.

1. Find each sample proportion: `=x1/n1` and `=x2/n2`
2. Find the pooled proportion: `=(x1+x2)/(n1+n2)`
3. Find the standard error: `=SQRT(pbar*(1-pbar)*(1/n1+1/n2))`
4. Find the test statistic: `=(phat1-phat2)/SE`
5. Find the p-value with `NORM.S.DIST`:
    * Right-tailed: `=1-NORM.S.DIST(z,TRUE)`
    * Left-tailed: `=NORM.S.DIST(z,TRUE)`
    * Two-tailed: `=2*(1-NORM.S.DIST(ABS(z),TRUE))`

For example, with $\bar p$ in B1, $n_1$ in B3, and $n_2$ in B4, the standard error formula would be `=SQRT(B1*(1-B1)*(1/B3+1/B4))`.

### Desmos
In [Desmos](www.desmos.com/calculator), type each formula in sequence, replacing the numbers with those from your problem:

$$\bar{p} = \frac{140+110}{250+230} \qquad SE = \sqrt{\bar{p}(1-\bar{p})\left(\frac{1}{250}+\frac{1}{230}\right)} \qquad z = \frac{0.56-0.478}{SE}$$

Find the critical value using the inverse-normal method from Lesson 18.1, and the p-value using the cumulative normal distribution method from Lesson 20.4. Compare the results to make your decision, exactly as in the example above.
