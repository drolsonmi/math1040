<head>
<title>23.1 Hypotheses of 2 Independent Samples</title>
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

# Lesson 23.1 Hypotheses of 2 Independent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.2.1 Setting up hypotheses for a difference of proportions (pages 242-244)

## Lesson
Just as Lesson 22 compared two independent means, we can also compare two independent **proportions** — for example, comparing the success rate of two different treatments, or the approval rate between two different cities.

### The Null and Alternate Hypotheses
Our default assumption is that there is **no difference** between the two population proportions:

$$H_0: p_1 = p_2 \qquad \text{(equivalently, } p_1 - p_2 = 0\text{)}$$

The alternate hypothesis again takes one of three forms:

| Research Question                  | Alternate Hypothesis | Test Type    |
| :--------------------------------- | :------------------: | :----------- |
| Is $p_1$ **greater than** $p_2$?   | $H_A: p_1 > p_2$     | Right-tailed |
| Is $p_1$ **less than** $p_2$?      | $H_A: p_1 < p_2$     | Left-tailed  |
| Is $p_1$ **different from** $p_2$? | $H_A: p_1 \ne p_2$   | Two-tailed   |

### The Pooled Proportion
Since $H_0$ assumes $p_1 = p_2$, we assume there is really just one common proportion shared by both groups. We estimate that common proportion by combining ("pooling") both samples together:

$$\bar{p} = \frac{x_1 + x_2}{n_1 + n_2}$$

where $x_1$ and $x_2$ are the number of successes in each sample. We'll use $\bar{p}$ (the pooled proportion) any time we need to check conditions or calculate a test statistic under the assumption that $H_0$ is true.

### Verifying the Conditions
Before comparing two proportions, we need to verify:
1. **Both samples are random**
2. **The two samples are independent of each other**
3. **The success-failure condition holds for both samples, using the pooled proportion:**

$$n_1\bar{p} \ge 10 \qquad n_1(1-\bar{p}) \ge 10 \qquad n_2\bar{p} \ge 10 \qquad n_2(1-\bar{p}) \ge 10$$

If all conditions hold, the sampling distribution of $\hat{p}_1 - \hat{p}_2$ is approximately normal, and we can proceed with a z-based test.

### Example

> A wellness organization wants to know if the proportion of adults who exercise regularly is different between City A and City B. A random sample of 250 adults in City A found that 140 exercise regularly. An independent random sample of 230 adults in City B found that 110 exercise regularly. Test at the 5% significance level.

**Identifying the information:**
* City A: $n_1 = 250$, $x_1 = 140$, so $\hat{p}_1 = 140/250 = 0.56$
* City B: $n_2 = 230$, $x_2 = 110$, so $\hat{p}_2 = 110/230 \approx 0.478$

**Setting up the hypotheses:**

$$H_0: p_1 = p_2 \qquad\qquad H_A: p_1 \ne p_2 \quad \text{(two-tailed)}$$

**Verifying the conditions:**
* Both samples are random — *stated in the problem*
* The two samples are independent — *different adults in two different cities*
* Pooled proportion: $\bar{p} = \dfrac{140+110}{250+230} = \dfrac{250}{480} \approx 0.521$
    * $n_1\bar{p} = 250(0.521) = 130.2 \ge 10$ ✓ and $n_1(1-\bar{p}) = 250(0.479) = 119.8 \ge 10$ ✓
    * $n_2\bar{p} = 230(0.521) = 119.8 \ge 10$ ✓ and $n_2(1-\bar{p}) = 230(0.479) = 110.2 \ge 10$ ✓

All conditions are satisfied, so we can proceed with a hypothesis test in Lesson 23.3.

## Practice
For each of the following questions, identify the two sample proportions, state both hypotheses, and verify the conditions.

1. A marketing team wants to know if customer satisfaction differs between two products. A random sample of 180 Product A customers found 126 satisfied. An independent random sample of 165 Product B customers found 90 satisfied. Test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/23_1_Solution1.md)
2. A public health department wants to know if a new smoking cessation program has a higher success rate than the standard program. A random sample of 140 participants in the new program found that 42 successfully quit smoking. An independent random sample of 150 participants in the standard program found that 27 successfully quit. Test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/23_1_Solution2.md)
3. A quality control manager wants to know if Machine A has a lower defect rate than Machine B. A random sample of 200 items from Machine A found 14 defective. An independent random sample of 220 items from Machine B found 24 defective. Test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/23_1_Solution3.md)
