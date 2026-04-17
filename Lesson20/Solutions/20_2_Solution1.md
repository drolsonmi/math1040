<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level (90% confidence level), test the claim that the average wait time is greater than 4 minutes.

## Solution
From the problem we get the following information:
* Null value: $$\mu_0 = 4$$
* Sample size: $$n = 35$$
* Sample mean: $$\bar{x} = 4.6$$
* Sample standard deviation: $$s = 1.2$$
* Confidence level: 90%

We will follow these steps:
1. Verify that the CLT is satisfied
2. State the hypotheses
3. Calculate the confidence interval
4. Compare to the null value

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **Yes** (stated in the problem)
* Is the sample large enough? **Yes** ($$n = 35 \ge 30$$)

The Central Limit Theorem holds.

**Step 2 — Hypotheses**

$$H_0: \mu = 4 \qquad\qquad H_A: \mu > 4$$

**Step 3 — Confidence Interval**

Since we do not have a population standard deviation ($$\sigma$$), we use the t-distribution with the `TInterval` function on the TI-84. With $$\bar{x} = 4.6$$, $$s = 1.2$$, $$n = 35$$, and a 90% confidence level, the calculator gives:

$$(4.257,\ 4.943)$$

**Step 4 — Compare to the null value**

The null value $$\mu_0 = 4$$ is **not** inside the confidence interval. Therefore, we can **reject the null hypothesis**.

**Conclusion:** There is enough evidence at the 5% significance level to support the claim that the average wait time is more than 4 minutes.

[Return back to Lesson 20.2](../20_2_HypTestAndConfInt.md#practice)
