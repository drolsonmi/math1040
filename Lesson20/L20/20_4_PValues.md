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
In Lesson 20.3, we made our decision by comparing a __test statistic__ to a __critical region__. There is a second, closely related way to make the same decision: the __p-value__.

#### What is a P-value?
The __p-value__ is the probability, *assuming the null hypothesis is true*, of getting a test statistic as extreme as (or more extreme than) the one we actually calculated from our sample.

In other words, the p-value answers the question: *"If the null hypothesis really is true, how unusual is our sample result?"* A __small__ p-value means our sample result would be very unusual if $$H_0$$ were true — which is evidence against $$H_0$$. A __large__ p-value means our sample result is not unusual at all under $$H_0$$ — which gives us no reason to doubt it.

#### Making a Decision with the P-value
We compare the p-value directly to our level of significance, $$\alpha$$:

* If $$p\text{-value} \le \alpha$$, we __reject the null hypothesis__ — the result is unusual enough to count as evidence against $$H_0$$.
* If $$p\text{-value} > \alpha$$, we __fail to reject the null hypothesis__ — the result isn't unusual enough to abandon our default assumption.

This is the exact same decision the critical region gives us — it's just expressed as a probability instead of a value on the number line. In fact, one always leads to the same conclusion as the other, because the critical value and the p-value are found from the exact same tail area, just used in opposite directions: the critical value converts $$\alpha$$ into a test statistic, while the p-value converts the test statistic into an area.

#### Calculating the P-value
The way we calculate the p-value depends on the type of test:

* __Right-tailed test__ ($$H_A: \mu > \mu_0$$): the p-value is the area to the *right* of the test statistic

$$p = P(Z > z)$$

* __Left-tailed test__ ($$H_A: \mu < \mu_0$$): the p-value is the area to the *left* of the test statistic

$$p = P(Z < z)$$

* __Two-tailed test__ ($$H_A: \mu \ne \mu_0$$): the p-value is *twice* the area beyond the test statistic (since evidence could show up on either side)

$$p = 2 \times P(Z > |z|)$$

#### Example
Let's return to the Snow College IQ example from Lesson 20.3:

> American mental abilities are often measured by an IQ test. The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

We already found the hypotheses and the test statistic in Lesson 20.3:

$$H_0: \mu = 100 \qquad\qquad H_A: \mu > 100 \qquad\qquad z \approx 2.656$$

This is a right-tailed test, so the p-value is the area to the right of $$z = 2.656$$:

$$p = P(Z > 2.656) \approx 0.0040$$

Since $$p \approx 0.0040$$ is less than $$\alpha = 0.05$$, we __reject the null hypothesis__ — the exact same conclusion we reached using the critical region in Lesson 20.3.

## Practice
Each of these problems reuses a scenario from Lesson 20.3. Instead of using the critical region, use the p-value to make your decision, and confirm that you reach the same conclusion.

1. A tire manufacturer claims their tires last, on average, 50,000 miles, with a population standard deviation of 4,000 miles. A random sample of 36 tires shows an average lifespan of 51,200 miles. At the 5% significance level, test the claim that the tires last *longer* than advertised, using the p-value.
    * After solving on your own, check the solution: <button popovertarget="Problem_1">Solution</button>
2. A pharmaceutical company claims a new drug brings average recovery time to 10 days, with a population standard deviation of 2.5 days. A random sample of 50 patients shows an average recovery time of 9.3 days. At the 1% significance level, test whether the true average recovery time is *different* from 10 days, using the p-value.
    * After solving on your own, see solution here <button popovertarget="Problem_2">Solution</button>
3. A factory claims it takes an average of 30 minutes to assemble a product, with a population standard deviation of 5 minutes. After a new training program, a random sample of 32 workers shows an average assembly time of 27.8 minutes. At the 5% significance level, test whether the new training has *reduced* the average assembly time, using the p-value.
    * After solving on your own, see solution here <button popovertarget="Problem_3">Solution</button>

<div popover id="Problem_1">

## Problem 20.4.1
A tire manufacturer claims their tires last, on average, __50,000 miles__, with a __population standard deviation of 4,000 miles__. A __random sample of 36 tires__ shows an __average lifespan of 51,200 miles__. At the __5% significance level__, test the claim that the tires last *longer* than advertised, using the p-value.

From Lesson 20.3, the hypotheses and test statistic are:

$$H_0: \mu = 50{,}000 \qquad\qquad H_A: \mu > 50{,}000 \qquad\qquad z \approx 1.80$$

This is a right-tailed test, so the p-value is the area to the right of $$z = 1.80$$:

$$p = P(Z > 1.80) \approx 0.0359$$

Since $$p \approx 0.0359$$ is less than $$\alpha = 0.05$$, we __reject the null hypothesis__.

There is enough evidence, at the 5% significance level, to conclude that the tires last longer than 50,000 miles on average. This matches our conclusion from Lesson 20.3.

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

## Problem 20.4.2
A pharmaceutical company claims a new drug brings average recovery time to __10 days__, with a __population standard deviation of 2.5 days__. A __random sample of 50 patients__ shows an __average recovery time of 9.3 days__. At the __1% significance level__, test whether the true average recovery time is *different* from 10 days, using the p-value.

From Lesson 20.3, the hypotheses and test statistic are:

$$H_0: \mu = 10 \qquad\qquad H_A: \mu \ne 10 \qquad\qquad z \approx -1.98$$

This is a two-tailed test, so the p-value is twice the area beyond $$|z| = 1.98$$:

$$p = 2 \times P(Z > 1.98) \approx 2 \times 0.0239 = 0.0478$$

Since $$p \approx 0.0478$$ is greater than $$\alpha = 0.01$$, we __fail to reject the null hypothesis__.

There is not enough evidence, at the 1% significance level, to conclude that the true average recovery time is different from 10 days. This matches our conclusion from Lesson 20.3.

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

## Problem 20.4.3
A factory claims it takes an average of __30 minutes__ to assemble a product, with a __population standard deviation of 5 minutes__. After a new training program, a __random sample of 32 workers__ shows an __average assembly time of 27.8 minutes__. At the __5% significance level__, test whether the new training has *reduced* the average assembly time, using the p-value.

From Lesson 20.3, the hypotheses and test statistic are:

$$H_0: \mu = 30 \qquad\qquad H_A: \mu < 30 \qquad\qquad z \approx -2.49$$

This is a left-tailed test, so the p-value is the area to the left of $$z = -2.49$$:

$$p = P(Z < -2.49) \approx 0.0064$$

Since $$p \approx 0.0064$$ is less than $$\alpha = 0.05$$, we __reject the null hypothesis__.

There is enough evidence, at the 5% significance level, to conclude that the new training program has reduced the average assembly time. This matches our conclusion from Lesson 20.3.

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>


## Technology

### TI-83/84
The built-in hypothesis test menu gives you the p-value directly, so you don't need to look anything up separately:
* Press `STAT`
* Select the `TESTS` menu
* Select `1:Z-Test...` if $$\sigma$$ is known, or `2:T-Test...` if it is not
* Choose `Stats`, then enter $$\mu_0$$, $$\sigma$$ (or $$s_x$$), $$\bar{x}$$, and $$n$$
* Choose the alternate hypothesis (`$$\ne \mu_0$$`, `$$<\mu_0$$`, or `$$>\mu_0$$`)
* Select "Calculate"

Note that the p-value appears on your TI-84 as `p=`. This is not to be confused with $$\hat{p}$$ which is your sample statistic, or the proportion of successes in your sample.

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
