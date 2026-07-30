<head>
<title>20.3 Critical Regions</title>
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

# Lesson 20.3 Critical Regions
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.3.3 Evaluating hypotheses with a significance level (pages 198–201)

## Lesson

In the previous lesson we used a confidence interval to judge whether the null hypothesis should be rejected. In practice, hypothesis testing uses a closely related idea: the **critical region** (also called the **rejection region**).

#### Significance Level

Recall from the confidence interval work that a 90% confidence level leaves 10% of the area in the tails. In hypothesis testing, that leftover tail probability is called the **significance level**, denoted $$\alpha$$.

$$\alpha = 1 - \text{Confidence Level}$$

The significance level is the probability of rejecting the null hypothesis when it is actually true (a "false positive"). Common choices are:

| Significance Level | Confidence Level |
|---|---|
| $$\alpha = 0.10$$ | 90% |
| $$\alpha = 0.05$$ | 95% |
| $$\alpha = 0.01$$ | 99% |

#### The Critical Value and Critical Region

From the significance level we find a **critical value** — a threshold on the standard normal (or t) distribution. Any test statistic that falls beyond the critical value is in the **critical region**, which means there is enough evidence to reject $$H_0$$.

The shape of the critical region depends on the **alternate hypothesis**:

| Alternate Hypothesis | Test Type | Critical Region |
|---|---|---|
| $$H_A: \mu > \mu_0$$ | Right-tailed | Right tail, area = $$\alpha$$ |
| $$H_A: \mu < \mu_0$$ | Left-tailed | Left tail, area = $$\alpha$$ |
| $$H_A: \mu \ne \mu_0$$ | Two-tailed | Both tails, area = $$\alpha/2$$ each |

#### Computing the Test Statistic

To place a sample result on the standard normal distribution, we convert the sample mean to a **z-score** (when $$\sigma$$ is known) or a **t-score** (when only $$s$$ is known).

**When $$\sigma$$ is known — z-test:**

$$z = \frac{\bar{x} - \mu_0}{\sigma / \sqrt{n}}$$

**When only $$s$$ is known — t-test ($$DF = n-1$$):**

$$t = \frac{\bar{x} - \mu_0}{s / \sqrt{n}}$$

#### Decision Rule

Once you have the test statistic and the critical value $$z_c$$ (or $$t_c$$):

* **Right-tailed:** Reject $$H_0$$ if $$z > z_c$$ (or $$t > t_c$$)
* **Left-tailed:** Reject $$H_0$$ if $$z < -z_c$$ (or $$t < -t_c$$)
* **Two-tailed:** Reject $$H_0$$ if $$|z| > z_c$$ (or $$|t| > t_c$$)

#### Example

> American mental abilities are often measured by an IQ test. The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

We have:
* $$\mu_0 = 100$$, $$\sigma = 15$$, $$n = 40$$, $$\bar{x} = 106.3$$, $$\alpha = 0.05$$
* $$H_0: \mu = 100 \qquad H_A: \mu > 100$$ (right-tailed)

**Verify the CLT:**
* Random sample? **Yes**
* $$n = 40 \ge 30$$? **Yes**

The CLT holds.

**Critical value:** For a right-tailed test with $$\alpha = 0.05$$, the critical value is $$z_c = 1.645$$.

**Test statistic:**

$$z = \frac{106.3 - 100}{15/\sqrt{40}} = \frac{6.3}{2.372} = 2.656$$

**Decision:** $$z = 2.656 > z_c = 1.645$$, so we **reject $$H_0$$**.

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that the average IQ of Snow College students is higher than the national average of 100.

## Practice
1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, use the critical region method to test the claim.
    * [After solving on your own, see solution here](Solutions/20_3_Solution1.md)

2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A random sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level.
    * [After solving on your own, see solution here](Solutions/20_3_Solution2.md)

3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. A random sample of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/20_3_Solution3.md)

## Technology
### TI-83/84
#### Finding a Critical z-value
* Press `2nd` → `[DISTR]`
* Select `3:invNorm(`
* For a **right-tailed** test at $$\alpha$$: enter `invNorm(1-α, 0, 1)`
* For a **left-tailed** test at $$\alpha$$: enter `invNorm(α, 0, 1)`
* For a **two-tailed** test at $$\alpha$$: enter `invNorm(α/2, 0, 1)` (take the absolute value)

#### Finding a Critical t-value
* Press `2nd` → `[DISTR]`
* Select `4:invT(`
* For a **right-tailed** test: enter `invT(1-α, df)`
* For a **left-tailed** test: enter `invT(α, df)`
* For a **two-tailed** test: enter `invT(α/2, df)` (take the absolute value)
