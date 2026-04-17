<head>
<title>21.3 Full Hypothesis Tests with 1 Sample of Categorical Data</title>
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

# Lesson 21.3 Full Hypothesis Tests with 1 Sample of Categorical Data
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.1.2 Hypothesis testing for a proportion (pages 237–241)

## Lesson

We now combine everything from Lessons 21.1 and 21.2 into a complete five-step hypothesis test for a single categorical variable. The structure is identical to the quantitative test in Lesson 20.5 — only the formula for the test statistic and the verification conditions change.

#### The Five Steps for a Proportion Test

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random?
* Is $$np_0 \ge 10$$ and $$n(1-p_0) \ge 10$$?
* Is the sample independent (less than 10% of the population)?

**Step 2 — State the Hypotheses**

$$H_0: p = p_0 \qquad H_A: p > p_0 \text{ or } p < p_0 \text{ or } p \ne p_0$$

**Step 3 — Compute the Test Statistic**

$$z = \frac{\hat{p} - p_0}{\sqrt{\dfrac{p_0(1-p_0)}{n}}}$$

**Step 4 — Find the Critical Value and/or P-Value**

| Test Type | Critical value | P-value |
|---|---|---|
| Right-tailed | $$z_c$$ | `normalcdf(z, 1E99, 0, 1)` |
| Left-tailed | $$-z_c$$ | `normalcdf(-1E99, z, 0, 1)` |
| Two-tailed | $$\pm z_c$$ | `2 × normalcdf(|z|, 1E99, 0, 1)` |

**Step 5 — Make a Decision and Write a Conclusion**

* Reject $$H_0$$ if the test statistic is in the critical region, or if $$p\text{-value} \le \alpha$$.
* Write a plain-language conclusion that directly answers the original question.

---

#### Example

> According to a national survey, 55% of teenagers say they use social media for more than 3 hours per day. A school counselor believes the rate at their school is different. They survey a random sample of 120 students and find that 78 use social media for more than 3 hours daily. Test at the 5% significance level.

**Step 1 — Verify the CLT**
* Random? **Yes**
* $$np_0 = 120(0.55) = 66 \ge 10$$ ✓ and $$n(1-p_0) = 120(0.45) = 54 \ge 10$$ ✓
* Independence: The school has far more than $$120 \times 10 = 1{,}200$$ students ✓

**Step 2 — Hypotheses**

$$\hat{p} = 78/120 = 0.65$$

The counselor believes the rate may be **different** from 55%.

$$H_0: p = 0.55 \qquad\qquad H_A: p \ne 0.55 \quad \text{(two-tailed)}$$

**Step 3 — Test Statistic**

$$SE = \sqrt{\frac{0.55(0.45)}{120}} = \sqrt{0.002063} = 0.04541$$

$$z = \frac{0.65 - 0.55}{0.04541} = \frac{0.10}{0.04541} = 2.202$$

**Step 4 — Critical Value and P-Value**

* Critical value (two-tailed, $$\alpha = 0.05$$): $$z_c = \pm 1.960$$
* P-value: `2 × normalcdf(2.202, 1E99, 0, 1)` $$\approx 2 \times 0.0138 = 0.0276$$

**Step 5 — Decision and Conclusion**

* $$|z| = 2.202 > z_c = 1.960$$ → **Reject $$H_0$$**
* $$p = 0.0276 \le \alpha = 0.05$$ → **Reject $$H_0$$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the proportion of students at this school who use social media more than 3 hours per day is different from the national rate of 55%.

---

## Practice
1. A pharmaceutical company claims that 70% of patients who take their medication experience significant improvement. A research group suspects the true rate is lower. In a clinical trial with a random sample of 150 patients, 96 experienced significant improvement. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/21_3_Solution1.md)

2. A university reports that 30% of its students are first-generation college students. A student affairs office believes the proportion may be different. They survey a random sample of 250 students and find 85 are first-generation students. Conduct a full hypothesis test at the 10% significance level.
    * [After solving on your own, see solution here](Solutions/21_3_Solution2.md)

3. A city council claims that 60% of residents approve of a new park development plan. An opposition group believes the approval rate is lower. A random survey of 180 residents finds that 99 approve. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/21_3_Solution3.md)

## Technology
### TI-83/84
#### 1-Proportion Z-Test
* `STAT` → `[TESTS]`
* `5:1-PropZTest`
* Enter:
  * $$p_0$$: the null value
  * $$x$$: count of successes in the sample
  * $$n$$: sample size
* Select the direction of $$H_A$$
* Select `Calculate`

The output shows the z-statistic, the p-value, $$\hat{p}$$, and $$n$$. Compare the p-value to $$\alpha$$ to make your decision.
