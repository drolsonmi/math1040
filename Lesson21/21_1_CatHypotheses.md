<head>
<title>21.1 Setup of Hypothesis Tests with 1 Sample of Categorical Data</title>
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

# Lesson 21.1 Setup of Hypothesis Tests with 1 Sample of Categorical Data
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 6.1 Inference for a single proportion (pages 234–241)

## Lesson

In Lesson 20, we performed hypothesis tests on **quantitative** data, where we compared a sample mean $$\bar{x}$$ to a null value $$\mu_0$$. Now we turn to **categorical** data, where our parameter of interest is a **proportion** rather than a mean.

#### The Parameter: Population Proportion

A proportion is the fraction of a population that has a particular characteristic. We write the true population proportion as $$p$$. In a sample of size $$n$$, the **sample proportion** is:

$$\hat{p} = \frac{x}{n}$$

where $$x$$ is the count of individuals in the sample with the characteristic of interest.

#### The Null and Alternate Hypotheses

Just as before, the **null hypothesis** asserts that the true proportion equals a specific null value $$p_0$$:

$$H_0: p = p_0$$

The **alternate hypothesis** takes one of three forms depending on the question being asked:

| Research Question | Alternate Hypothesis | Test Type |
|---|---|---|
| Is the proportion **greater than** $$p_0$$? | $$H_A: p > p_0$$ | Right-tailed |
| Is the proportion **less than** $$p_0$$? | $$H_A: p < p_0$$ | Left-tailed |
| Is the proportion **different from** $$p_0$$? | $$H_A: p \ne p_0$$ | Two-tailed |

#### Verifying the Central Limit Theorem for Proportions

Before we can use the normal distribution to model $$\hat{p}$$, three conditions must be met:

1. **Random sample:** The sample must be collected randomly.
2. **Success-failure condition:** Both $$np_0 \ge 10$$ and $$n(1-p_0) \ge 10$$ must hold. (Note: we use $$p_0$$, not $$\hat{p}$$, because we are testing under the assumption that $$H_0$$ is true.)
3. **Independence:** The sample size is less than 10% of the population (usually safe to assume unless stated otherwise).

#### Example

> A polling organization reports that 45% of U.S. adults support a particular new policy. A local advocacy group believes that support in their city is higher than the national rate. They survey a random sample of 200 city residents and find that 102 of them support the policy. At the 5% significance level, is there evidence that support in the city is higher than 45%?

**Identifying the information:**
* Null value: $$p_0 = 0.45$$
* Sample size: $$n = 200$$
* Number of successes: $$x = 102$$
* Sample proportion: $$\hat{p} = 102/200 = 0.51$$

**Setting up the hypotheses:**

The group believes support is **higher** than the national rate.

$$H_0: p = 0.45 \qquad\qquad H_A: p > 0.45 \quad \text{(right-tailed)}$$

**Verifying the CLT:**
* Random sample? **Yes** (stated in the problem)
* Success-failure: $$np_0 = 200(0.45) = 90 \ge 10$$ ✓ and $$n(1-p_0) = 200(0.55) = 110 \ge 10$$ ✓
* Independence: A city has far more than $$200 \times 10 = 2{,}000$$ adults ✓

The CLT holds — we can proceed with the hypothesis test in the next lesson.

## Practice
For each of the following questions, identify the null value, state both hypotheses, and verify the Central Limit Theorem.

1. A pharmaceutical company claims that 70% of patients who take their medication experience significant improvement. A research group suspects the true rate is lower. In a clinical trial with a random sample of 150 patients, 96 experienced significant improvement. At the 5% significance level, test the company's claim.
    * [After solving on your own, see solution here](Solutions/21_1_Solution1.md)

2. A university reports that 30% of its students are first-generation college students. A student affairs office believes the proportion may be different from the reported value. They randomly survey 250 students and find that 85 are first-generation students. Test at the 10% significance level.
    * [After solving on your own, see solution here](Solutions/21_1_Solution2.md)

3. A city council claims that 60% of residents approve of a new park development plan. An opposition group believes the approval rate is lower. A random survey of 180 residents finds that 99 approve. Test at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/21_1_Solution3.md)
