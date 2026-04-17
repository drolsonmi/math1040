<head>
<title>21.2 Calculating Critical Regions and P-Values for Proportions</title>
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

# Lesson 21.2 Calculating Critical Regions and P-Values for Proportions
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.1.2 Hypothesis testing for a proportion (pages 237–241)

## Lesson

Now that we know how to set up a hypothesis test for a proportion, we need to calculate the **test statistic**, then use it to find the **critical value** or **p-value**. The procedure mirrors what we did for means in Lessons 20.3–20.4, but uses a different test statistic formula.

#### The Standard Error of a Proportion

When testing a proportion, we assume $$H_0$$ is true, so we use $$p_0$$ (not $$\hat{p}$$) to calculate the **standard error**:

$$SE = \sqrt{\frac{p_0(1-p_0)}{n}}$$

#### The Test Statistic

The test statistic for a proportion is always a **z-score** (not a t-score), because we are using the normal approximation to the sampling distribution of $$\hat{p}$$:

$$z = \frac{\hat{p} - p_0}{SE} = \frac{\hat{p} - p_0}{\sqrt{\dfrac{p_0(1-p_0)}{n}}}$$

#### Critical Values

Because we always use the z-distribution for proportions, the critical values come from the standard normal table:

| Test Type | Critical Value |
|---|---|
| Right-tailed | $$z_c$$ such that $$P(Z > z_c) = \alpha$$ |
| Left-tailed | $$-z_c$$ such that $$P(Z < -z_c) = \alpha$$ |
| Two-tailed | $$\pm z_c$$ such that $$P(Z > z_c) = \alpha/2$$ |

Common critical values:

| $$\alpha$$ | Right/Left-tailed $$z_c$$ | Two-tailed $$z_c$$ |
|---|---|---|
| 0.10 | 1.282 | 1.645 |
| 0.05 | 1.645 | 1.960 |
| 0.01 | 2.326 | 2.576 |

#### P-Values

As with the t-test, the p-value is the tail area beyond the observed test statistic:

| Test Type | P-value |
|---|---|
| Right-tailed | $$P(Z > z)$$ |
| Left-tailed | $$P(Z < z)$$ |
| Two-tailed | $$2 \times P(Z > \vert z\vert)$$ |

On the TI-84, use `normalcdf` since we are always working with the z-distribution.

#### Example

> A polling organization reports that 45% of U.S. adults support a particular new policy. An advocacy group surveys a random sample of 200 city residents and finds that 102 support the policy. At the 5% significance level, is there evidence that city support is higher than 45%?

From Lesson 21.1:
* $$p_0 = 0.45$$, $$n = 200$$, $$\hat{p} = 0.51$$
* $$H_0: p = 0.45 \qquad H_A: p > 0.45$$ (right-tailed)
* CLT verified ✓

**Standard Error:**

$$SE = \sqrt{\frac{0.45(0.55)}{200}} = \sqrt{\frac{0.2475}{200}} = \sqrt{0.0012375} = 0.03518$$

**Test Statistic:**

$$z = \frac{0.51 - 0.45}{0.03518} = \frac{0.06}{0.03518} = 1.706$$

**Critical Value** (right-tailed, $$\alpha = 0.05$$): $$z_c = 1.645$$

**P-value:** `normalcdf(1.706, 1E99, 0, 1)` $$\approx 0.0440$$

**Decision:**
* $$z = 1.706 > z_c = 1.645$$ → **Reject $$H_0$$**
* $$p = 0.0440 \le \alpha = 0.05$$ → **Reject $$H_0$$**

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that support in the city is higher than the national rate of 45%.

## Practice
1. A pharmaceutical company claims that 70% of patients who take their medication experience significant improvement. A research group suspects the true rate is lower. In a clinical trial with a random sample of 150 patients, 96 experienced significant improvement. At the 5% significance level, find the test statistic and the p-value.
    * [After solving on your own, see solution here](Solutions/21_2_Solution1.md)

2. A university reports that 30% of its students are first-generation college students. A student affairs office believes the proportion may be different. They survey a random sample of 250 students and find that 85 are first-generation students. At the 10% significance level, find the test statistic and the p-value.
    * [After solving on your own, see solution here](Solutions/21_2_Solution2.md)

3. A city council claims that 60% of residents approve of a new park development plan. An opposition group believes the approval rate is lower. A random survey of 180 residents finds that 99 approve. At the 5% significance level, find the test statistic and the p-value.
    * [After solving on your own, see solution here](Solutions/21_2_Solution3.md)

## Technology
### TI-83/84
#### P-value from a z-test statistic (proportions)
Because the test statistic for proportions is a z-score, use `normalcdf`:
* **Right-tailed:** `normalcdf(z, 1E99, 0, 1)`
* **Left-tailed:** `normalcdf(-1E99, z, 0, 1)`
* **Two-tailed:** `2 × normalcdf(|z|, 1E99, 0, 1)`

#### Running a Full 1-Proportion Z-Test directly
* `STAT` → `[TESTS]`
* `5:1-PropZTest`
* Enter $$p_0$$, $$x$$ (count of successes), and $$n$$
* Select the direction of $$H_A$$ ($$\ne$$, $$<$$, or $$>$$)
* Select `Calculate`

The calculator returns the z-test statistic and the p-value directly.
