<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level (98% confidence level).

## Solution
From the problem we get the following information:
* Null value: $$\mu_0 = 20$$
* Sample size: $$n = 55$$
* Sample mean: $$\bar{x} = 18.7$$
* Sample standard deviation: $$s = 2.5$$
* Confidence level: 98%

We will follow these steps:
1. Verify that the CLT is satisfied
2. State the hypotheses
3. Calculate the confidence interval
4. Compare to the null value

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes** (stated in the problem)
* Is the sample large enough? **Yes** ($$n = 55 \ge 30$$)

The Central Limit Theorem holds.

**Step 2 — Hypotheses**

$$H_0: \mu = 20 \qquad\qquad H_A: \mu < 20$$

**Step 3 — Confidence Interval**

Since we do not have a population standard deviation ($$\sigma$$), we use the t-distribution with the `TInterval` function on the TI-84. With $$\bar{x} = 18.7$$, $$s = 2.5$$, $$n = 55$$, and a 98% confidence level, the calculator gives:

$$(17.892,\ 19.508)$$

**Step 4 — Compare to the null value**

The null value $$\mu_0 = 20$$ is **not** inside the confidence interval. Therefore, we can **reject the null hypothesis**.

**Conclusion:** There is enough evidence at the 1% significance level to support the claim that the average battery life is less than 20 hours.

[Return back to Lesson 20.2](../20_2_HypTestAndConfInt.md#practice)
