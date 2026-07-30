<head>
<title>20.5 Full Hypothesis Tests with 1 Sample of Quantitative Data</title>
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

# Lesson 20.5 Full Hypothesis Tests with 1 Sample of Quantitative Data
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.3.3 – 5.3.5 (pages 198–206)
* 7.1.4 One sample t-tests (pages 281–282)

## Lesson

Now that we have all the individual pieces, we can put them together into a complete hypothesis test. Every hypothesis test for a single sample of quantitative data follows the same five-step procedure.

#### The Five Steps of a Hypothesis Test

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random?
* Is $$n \ge 30$$, OR is the population normally distributed?

If the CLT does not hold, stop — the test is not valid.

**Step 2 — State the Hypotheses**

Write both the null and alternate hypothesis. Identify whether the test is left-tailed, right-tailed, or two-tailed.

$$H_0: \mu = \mu_0 \qquad H_A: \mu > \mu_0 \text{ or } \mu < \mu_0 \text{ or } \mu \ne \mu_0$$

**Step 3 — Compute the Test Statistic**

If $$\sigma$$ is known, use the z-test:

$$z = \frac{\bar{x} - \mu_0}{\sigma / \sqrt{n}}$$

If only $$s$$ is known, use the t-test with $$DF = n - 1$$:

$$t = \frac{\bar{x} - \mu_0}{s / \sqrt{n}}$$

**Step 4 — Find the Critical Value and/or P-Value**

* **Critical value:** Use the significance level $$\alpha$$ and the tail direction to find $$z_c$$ or $$t_c$$.
* **P-value:** Find the tail probability beyond the test statistic.
  * Right-tailed: $$p = P(T > t)$$
  * Left-tailed: $$p = P(T < t)$$
  * Two-tailed: $$p = 2 \cdot P(T > |t|)$$

**Step 5 — Make a Decision and Write a Conclusion**

* If test statistic is in the critical region, OR if $$p \le \alpha$$: **Reject $$H_0$$**
* Otherwise: **Fail to reject $$H_0$$**

Always write a conclusion in plain language that answers the original question.

---

#### Example

> A car manufacturer claims its new hybrid model averages 50 miles per gallon (mpg) on the highway. An independent testing organization believes the true average is different from the claim. They test a random sample of 36 vehicles and find a sample mean of 48.3 mpg and a sample standard deviation of 4.8 mpg. At the 5% significance level, test the manufacturer's claim.

**Step 1 — Verify the CLT**
* Random sample? **Yes**
* $$n = 36 \ge 30$$? **Yes**

The CLT holds.

**Step 2 — Hypotheses**

The claim is 50 mpg; the testers believe it could be **different** (either direction).

$$H_0: \mu = 50 \qquad\qquad H_A: \mu \ne 50 \quad \text{(two-tailed)}$$

**Step 3 — Test Statistic**

No $$\sigma$$ given, so use the t-test with $$DF = 35$$:

$$t = \frac{48.3 - 50}{4.8/\sqrt{36}} = \frac{-1.7}{0.8} = -2.125$$

**Step 4 — Critical Value and P-Value**

* Critical value (two-tailed, $$\alpha = 0.05$$, $$DF = 35$$): $$t_c = \pm 2.030$$
* P-value: $$p = 2 \times P(T > 2.125) \approx 2 \times 0.0205 = 0.0410$$

On TI-84: `2 × tcdf(2.125, 1E99, 35)` $$\approx 0.0410$$

**Step 5 — Decision and Conclusion**

* Critical region: $$|t| = 2.125 > t_c = 2.030$$ → **Reject $$H_0$$**
* P-value: $$p = 0.0410 \le \alpha = 0.05$$ → **Reject $$H_0$$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the true average fuel economy of the hybrid model is different from the claimed 50 mpg.

---

## Practice
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/20_5_Solution1.md)

2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A random sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a full hypothesis test at the 1% significance level.
    * [After solving on your own, see solution here](Solutions/20_5_Solution2.md)

3. A hospital administrator claims the average length of stay for patients after a routine surgery is 3.5 days. A quality-improvement team suspects the average may be different. They review a random sample of 45 patient records and find a mean stay of 3.9 days with a standard deviation of 1.1 days. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/20_5_Solution3.md)

## Technology
### TI-83/84
#### Running a Full T-Test
* `STAT` → `[TESTS]`
* `2:T-Test`
* Set `Inpt` to `Stats`
* Enter $$\mu_0$$, $$\bar{x}$$, $$s$$, and $$n$$
* Select the tail direction ($$\ne$$, $$<$$, or $$>$$) to match $$H_A$$
* Select `Calculate`

The calculator returns the test statistic $$t$$, the p-value $$p$$, and the sample statistics. Compare $$p$$ to $$\alpha$$ to make your decision.

If $$\sigma$$ is known, use `1:Z-Test` instead and enter $$\sigma$$ rather than $$s$$.
