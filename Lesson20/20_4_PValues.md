<head>
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

# Lesson 20.4 P-Values
## Reading

## Lesson
## Lesson
In Lesson 20.3, we made our decision by comparing a __test statistic__ to a __critical region__. There is a second, closely related way to make the same decision: the __p-value__.

#### What is a P-value?
The __p-value__ is the probability, *assuming the null hypothesis is true*, of getting a test statistic as extreme as (or more extreme than) the one we actually calculated from our sample.

In other words, the p-value answers the question: *"If the null hypothesis really is true, how unusual is our sample result?"* A __small__ p-value means our sample result would be very unusual if $H_0$ were true — which is evidence against $H_0$. A __large__ p-value means our sample result is not unusual at all under $H_0$ — which gives us no reason to doubt it.

#### Making a Decision with the P-value
We compare the p-value directly to our level of significance, $\alpha$:

* If $p\text{-value} \le \alpha$, we __reject the null hypothesis__ — the result is unusual enough to count as evidence against $H_0$.
* If $p\text{-value} > \alpha$, we __fail to reject the null hypothesis__ — the result isn't unusual enough to abandon our default assumption.

This is the exact same decision the critical region gives us — it's just expressed as a probability instead of a value on the number line. In fact, one always leads to the same conclusion as the other, because the critical value and the p-value are found from the exact same tail area, just used in opposite directions: the critical value converts $\alpha$ into a test statistic, while the p-value converts the test statistic into an area.

#### Calculating the P-value
The way we calculate the p-value depends on the type of test:

* __Right-tailed test__ ($H_A: \mu > \mu_0$): the p-value is the area to the *right* of the test statistic

$$p = P(Z > z)$$

* __Left-tailed test__ ($H_A: \mu < \mu_0$): the p-value is the area to the *left* of the test statistic

$$p = P(Z < z)$$

* __Two-tailed test__ ($H_A: \mu \ne \mu_0$): the p-value is *twice* the area beyond the test statistic (since evidence could show up on either side)

$$p = 2 \times P(Z > |z|)$$

#### Example
Let's return to the Snow College IQ example from Lesson 20.3:

> American mental abilities are often measured by an IQ test. The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

We already found the hypotheses and the test statistic in Lesson 20.3:

$$H_0: \mu = 100 \qquad\qquad H_A: \mu > 100 \qquad\qquad z \approx 2.656$$

This is a right-tailed test, so the p-value is the area to the right of $z = 2.656$:

$$p = P(Z > 2.656) \approx 0.0040$$

Since $p \approx 0.0040$ is less than $\alpha = 0.05$, we __reject the null hypothesis__ — the exact same conclusion we reached using the critical region in Lesson 20.3.

## Practice
For each of the following questions (same questions as in 20.2 and 20.3), state the correct hypotheses and determine the level of significance. Then use the p-value to make your decision and confirm that you reach the same conclusion as you did in 20.3.

1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, use the critical region method to test the claim.
    * [After solving on your own, see solution here](./Solutions/20_4_Solution1.md)
2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A random sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/20_4_Solution2.md)
3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. A random sample of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/20_4_Solution3.md)


## Technology

### TI-83/84
The built-in hypothesis test menu gives you the p-value directly, so you don't need to look anything up separately:
* Press `STAT`
* Select the `TESTS` menu
* Select `1:Z-Test...` if $\sigma$ is known, or `2:T-Test...` if it is not
* Choose `Stats`, then enter $\mu_0$, $\sigma$ (or $s_x$), $\bar{x}$, and $n$
* Choose the alternate hypothesis (`$\ne \mu_0$`, `$<\mu_0$`, or `$>\mu_0$`)
* Select "Calculate"

Note that the p-value appears on your TI-84 as `p=`. This is not to be confused with $\hat{p}$ which is your sample statistic, or the proportion of successes in your sample.

### Excel
Use `NORM.S.DIST` to find the area under the standard normal curve, or `T.DIST`/`T.DIST.2T` if you are working with a t-score.

* __Right-tailed test:__ type `=1-NORM.S.DIST(z,TRUE)`, replacing `z` with your test statistic or the cell that contains it
* __Left-tailed test:__ type `=NORM.S.DIST(z,TRUE)`
* __Two-tailed test:__ type `=2*(1-NORM.S.DIST(ABS(z),TRUE))`

For example, if your test statistic is in cell B1 and you have a right-tailed test, you would type `=1-NORM.S.DIST(B1,TRUE)`.

### Desmos
In [Desmos](www.desmos.com/calculator), you can find the p-value using the normal distribution's cumulative density directly, or by typing the area formula:

$$p = 1 - \text{normaldist}(0,1).\text{cdf}(2.656)$$

Replace `2.656` with your own test statistic, and adjust for a left-tailed (use `.cdf(z)` directly) or two-tailed test (multiply the one-tailed result by 2) as needed.
