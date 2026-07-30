<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. The educator believes the new method may lead to a different average score. A class of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level (95% confidence level).

## Solution
From the problem we get the following information:
* Null value: $\mu_0 = 75$
* Sample size: $n = 40$
* Sample mean: $\bar{x} = 78.2$
* Sample standard deviation: $s = 6.3$
* Confidence level: 95%

We will follow these steps:
1. Verify that the CLT is satisfied
2. State the hypotheses
3. Calculate the confidence interval
4. Compare to the null value

**Step 1 — Verify the Central Limit Theorem**
* Is the sample random? **No** — the problem describes a class (a convenience sample), not a random sample.
* Is the sample large enough? **Yes** ($n = 40 \ge 30$)

<font color='red'>The Central Limit Theorem does **not** fully hold because the sample is not random. Technically, we should stop here.</font> However, for practice purposes we will proceed anyway.

**Step 2 — Hypotheses**

$$H_0: \mu = 75 \qquad\qquad H_A: \mu \ne 75$$

**Step 3 — Confidence Interval**

Since we do not have a population standard deviation ($\sigma$), we use the t-distribution with the `TInterval` function on the TI-84. With $\bar{x} = 78.2$, $s = 6.3$, $n = 40$, and a 95% confidence level, the calculator gives:

$$(76.185,\ 80.215)$$

**Step 4 — Compare to the null value**

The null value $\mu_0 = 75$ is **not** inside the confidence interval. Therefore, we **reject the null hypothesis**.

**Conclusion:** Assuming the CLT held, there would be enough evidence at the 5% significance level to suggest that the new teaching method leads to a different average score than 75.

[Return back to Lesson 20.2](../20_2_HypTestAndConfInt.md#practice)
