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

# Lesson 20.3 Critical Regions
## Reading

## Lesson

#### Level of Significance
In Lesson 20.2, we used a confidence level to build a confidence interval and compare it to the null value. In hypothesis testing, we use the flip side of that same number: the __level of significance__, denoted $$\alpha$$ (the Greek letter "alpha").

$$\alpha = 1 - \text{Confidence Level}$$

The level of significance is the probability that we are willing to accept of __rejecting a true null hypothesis__ — in other words, the risk we're willing to take of concluding there's an effect when there really isn't one. Common choices are:

| Confidence Level | Level of Significance ($$\alpha$$) |
| :---------------: | :-----------------------------: |
| 90% | 0.10 |
| 95% | 0.05 |
| 99% | 0.01 |

A smaller $$\alpha$$ means we are demanding stronger evidence before we are willing to reject the null hypothesis. Just as we chose a confidence level before building a confidence interval, we choose (or are given) a level of significance before running a hypothesis test.

#### Left-tailed, Right-tailed, and Two-tailed tests
We saw in 20.1 that there are 3 different possible Alternate Hypotheses we can choose from:
1. The true value is greater than the null value

$$H_A: \mu > \mu_0$$

2. The true value is less than the null value

$$H_A: \mu < \mu_0$$

3. The true value is different from the null value

$$H_A: \mu \ne \mu_0$$

Each of these corresponds to a different shape for our test, based on where the evidence *against* $$H_0$$ would show up on the distribution:

* If $$H_A: \mu > \mu_0$$, the evidence against $$H_0$$ would appear as an unusually *large* sample value. This is a __right-tailed test__, and all of $$\alpha$$ goes in the right tail.
* If $$H_A: \mu < \mu_0$$, the evidence against $$H_0$$ would appear as an unusually *small* sample value. This is a __left-tailed test__, and all of $$\alpha$$ goes in the left tail.
* If $$H_A: \mu \ne \mu_0$$, the evidence against $$H_0$$ could appear as *either* an unusually large or unusually small sample value. This is a __two-tailed test__, and $$\alpha$$ is split evenly between both tails ($$\alpha/2$$ in each tail).

This is exactly the same idea we used with confidence intervals — a confidence interval is always "two-tailed" because it looks for values both above and below the sample statistic. A one-tailed hypothesis test, on the other hand, only worries about evidence in one direction, so the *entire* level of significance is placed in that one tail. This is why the critical values you find for a one-tailed test at a given $$\alpha$$ are not the same as the ones you found for a confidence interval at $$1-\alpha$$ confidence — the confidence interval splits its "leftover" area into both tails, while a one-tailed test does not.

#### The Critical Region
The __critical region__ (also called the __rejection region__) is the set of test statistic values that are unusual enough, assuming the null hypothesis is true, that we would reject $$H_0$$ in favor of $$H_A$$. The boundary of the critical region is marked by the __critical value__ — the same type of z-score (or t-score) we used to build confidence intervals.

* For a __right-tailed test__, the critical region is everything to the *right* of the critical value: $$z > z_c$$
* For a __left-tailed test__, the critical region is everything to the *left* of the critical value: $$z < -z_c$$
* For a __two-tailed test__, the critical region is split into both tails: $$z < -z_c \text{ or } z > z_c$$

The critical value itself is found the same way we found it for confidence intervals, using the level of significance instead of $$1 -$$ confidence level to find the appropriate area.

#### Using the Test Statistic and the Critical Region
Once we know the critical region, we calculate a __test statistic__ from our sample. The test statistic measures how many standard errors our sample result is away from the null value:

$$z = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}} \qquad\qquad \text{or} \qquad\qquad t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}$$

We use the z-score when the population standard deviation ($$\sigma$$) is known, and the t-score when we only have the sample standard deviation ($$s$$), exactly as we did for confidence intervals.

Once we've calculated the test statistic, the decision is simple:
* If the test statistic falls __inside the critical region__, we have unusual enough evidence to __reject the null hypothesis__.
* If the test statistic does __not__ fall inside the critical region, we __fail to reject the null hypothesis__ — we simply don't have enough evidence to abandon our default assumption.

Notice that we never say we "accept" the null hypothesis. Just like the jury in Lesson 20.1 doesn't declare someone "innocent" — only "not guilty" (not enough evidence to convict) — we don't declare $$H_0$$ true. We only ever say we don't have enough evidence to reject it.

#### Example
Let's revisit and solve the example brought up in 20.1:

> American mental abilities are often measured by an IQ test.  The IQ distribution is normal with a mean of 100 and a population standard deviation of 15. A random sample of 40 Snow College students is taken and they have an average IQ of 106.3. Can we say with a 5% level of significance that the true average IQ of Snow College students is higher than the nation?

To solve, let's do the following:
1. Make sure the Central Limit Theorem (CLT) holds
2. Define our hypotheses
3. Find the critical region
4. Find the test statistic

__1. Central Limit Theorem__
* The sample is random
* The population (IQ scores) is normally distributed, so this condition is satisfied regardless of sample size

Both conditions are satisfied, so the CLT holds and we may continue.

__2. Hypotheses__

Comparing to the national average of 100, and testing whether Snow College's average is *higher*, this is a right-tailed test:

$$H_0: \mu = 100 \qquad\qquad H_A: \mu > 100$$

__3. Critical Region__

We are given $$\alpha = 0.05$$. Since this is a right-tailed test, all of $$\alpha$$ goes in the right tail. The critical value is

$$z_c = 1.645$$

so the critical region is

$$z > 1.645$$

__4. Test Statistic__

Since we know the population standard deviation ($$\sigma = 15$$), we use a z-score:

$$z = \frac{\bar{x}-\mu_0}{\sigma/\sqrt{n}} = \frac{106.3 - 100}{15/\sqrt{40}} = \frac{6.3}{2.372} \approx 2.656$$

__5. Decision__

Our test statistic, $$z \approx 2.656$$, falls inside the critical region ($$z > 1.645$$). So, we __reject the null hypothesis__.

There is enough evidence, at the 5% level of significance, to conclude that the true average IQ of Snow College students is higher than the national average. This matches exactly what we found using the confidence interval in Lesson 20.2!

## Practice
1. A tire manufacturer claims their tires last, on average, 50,000 miles. Based on years of production data, the population standard deviation is known to be 4,000 miles. A random sample of 36 tires shows an average lifespan of 51,200 miles. At the 5% significance level, test the claim that the tires last *longer* than advertised.
    * After solving on your own, check the solution: <button popovertarget="Problem_1">Solution</button>
2. A pharmaceutical company claims a new drug brings average recovery time to 10 days, with a population standard deviation of 2.5 days (based on clinical trial history). A random sample of 50 patients using the drug shows an average recovery time of 9.3 days. At the 1% significance level, test whether the true average recovery time is *different* from 10 days.
    * After solving on your own, see solution here <button popovertarget="Problem_2">Solution</button>
3. A factory claims it takes an average of 30 minutes to assemble a product, with a population standard deviation of 5 minutes. After introducing a new training program, a random sample of 32 workers shows an average assembly time of 27.8 minutes. At the 5% significance level, test whether the new training has *reduced* the average assembly time.
    * After solving on your own, see solution here <button popovertarget="Problem_3">Solution</button>

<div popover id="Problem_1">

## Problem 20.3.1
A tire manufacturer claims their tires last, on average, __50,000 miles__. Based on years of production data, the __population standard deviation is known to be 4,000 miles__. A __random sample of 36 tires__ shows an __average lifespan of 51,200 miles__. At the __5% significance level__, test the claim that the tires last *longer* than advertised.

__1. Central Limit Theorem__
* The sample is random
* The sample is large enough ($$n = 36 > 30$$)

Both conditions are satisfied.

__2. Hypotheses__

We are testing whether the true average is *longer* than the claimed 50,000 miles, so this is a right-tailed test:

$$H_0: \mu = 50{,}000 \qquad\qquad H_A: \mu > 50{,}000$$

__3. Critical Region__

$$\alpha = 0.05$$, right-tailed, so $$z_c = 1.645$$ and the critical region is $$z > 1.645$$.

__4. Test Statistic__

The population standard deviation is known, so we use a z-score:

$$z = \frac{51{,}200 - 50{,}000}{4{,}000/\sqrt{36}} = \frac{1{,}200}{666.67} \approx 1.80$$

__5. Decision__

Since $$z \approx 1.80$$ falls inside the critical region ($$z > 1.645$$), we __reject the null hypothesis__.

There is enough evidence, at the 5% significance level, to conclude that the tires last longer than 50,000 miles on average.

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

## Problem 20.3.2
A pharmaceutical company claims a new drug brings average recovery time to __10 days__, with a __population standard deviation of 2.5 days__. A __random sample of 50 patients__ shows an __average recovery time of 9.3 days__. At the __1% significance level__, test whether the true average recovery time is *different* from 10 days.

__1. Central Limit Theorem__
* The sample is random
* The sample is large enough ($$n = 50 > 30$$)

Both conditions are satisfied.

__2. Hypotheses__

We are testing whether the true average is *different* from 10 days (could be higher or lower), so this is a two-tailed test:

$$H_0: \mu = 10 \qquad\qquad H_A: \mu \ne 10$$

__3. Critical Region__

$$\alpha = 0.01$$, two-tailed, so $$\alpha/2 = 0.005$$ in each tail. The critical value is $$z_c = 2.576$$, and the critical region is $$z < -2.576 \text{ or } z > 2.576$$.

__4. Test Statistic__

The population standard deviation is known, so we use a z-score:

$$z = \frac{9.3 - 10}{2.5/\sqrt{50}} = \frac{-0.7}{0.354} \approx -1.98$$

__5. Decision__

Since $$z \approx -1.98$$ does *not* fall inside the critical region ($$z < -2.576$$ or $$z > 2.576$$), we __fail to reject the null hypothesis__.

There is not enough evidence, at the 1% significance level, to conclude that the true average recovery time is different from 10 days.

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

## Problem 20.3.3
A factory claims it takes an average of __30 minutes__ to assemble a product, with a __population standard deviation of 5 minutes__. After introducing a new training program, a __random sample of 32 workers__ shows an __average assembly time of 27.8 minutes__. At the __5% significance level__, test whether the new training has *reduced* the average assembly time.

__1. Central Limit Theorem__
* The sample is random
* The sample is large enough ($$n = 32 > 30$$)

Both conditions are satisfied.

__2. Hypotheses__

We are testing whether the true average is *less than* 30 minutes, so this is a left-tailed test:

$$H_0: \mu = 30 \qquad\qquad H_A: \mu < 30$$

__3. Critical Region__

$$\alpha = 0.05$$, left-tailed, so the critical value is $$z_c = -1.645$$, and the critical region is $$z < -1.645$$.

__4. Test Statistic__

The population standard deviation is known, so we use a z-score:

$$z = \frac{27.8 - 30}{5/\sqrt{32}} = \frac{-2.2}{0.884} \approx -2.49$$

__5. Decision__

Since $$z \approx -2.49$$ falls inside the critical region ($$z < -1.645$$), we __reject the null hypothesis__.

There is enough evidence, at the 5% significance level, to conclude that the new training program has reduced the average assembly time.

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>


## Technology

### TI-83/84
You can find the critical value the same way we did for confidence intervals:
* Press `2ND`, then `VARS` to open the `DISTR` menu
* Select `invNorm(`
* For a right-tailed test, enter the area to the left of the critical value (i.e., $$1-\alpha$$). For a left-tailed test, enter $$\alpha$$ directly. For a two-tailed test, enter $$1-\alpha/2$$ for the positive critical value (the negative critical value is the same number, negated).

You can find the test statistic directly using the built-in hypothesis test menu:
* Press `STAT`
* Select the `TESTS` menu
* Select `1:Z-Test...` if $$\sigma$$ is known, or `2:T-Test...` if it is not
* Choose `Stats`, then enter $$\mu_0$$, $$\sigma$$ (or $$s_x$$), $$\bar{x}$$, and $$n$$
* Choose the alternate hypothesis (`$$\ne \mu_0$$`, `$$<\mu_0$$`, or `$$>\mu_0$$`)
* Select "Calculate"

The calculator returns the test statistic (`z` or `t`). Compare this to the critical value(s) you found to make your decision.

### Excel
__Critical Value:__ Just as with confidence intervals, use `NORM.S.INV` for a z critical value, or `T.INV` for a t critical value.
* For a right-tailed test at $$\alpha = 0.05$$: type `=NORM.S.INV(0.95)` (enter the area to the *left* of the critical value, $$1-\alpha$$)
* For a two-tailed test at $$\alpha = 0.05$$: type `=NORM.S.INV(0.975)` (area to the left of the *positive* critical value, $$1-\alpha/2$$)

__Test Statistic:__ Build the formula directly from the pieces.
* In a cell, type `=(` followed by the cell with $$\bar{x}$$, `-`, the cell with $$\mu_0$$, `)/(`, the cell with $$\sigma$$ (or $$s$$), `/SQRT(`, the cell with $$n$$, `))`
  * For example, if $$\bar{x}$$ is in B1, $$\mu_0$$ is in B2, $$\sigma$$ is in B3, and $$n$$ is in B4, type `=(B1-B2)/(B3/SQRT(B4))`
* Press `Enter`

Compare the resulting value to your critical value(s) to make your decision.

### Desmos
In [Desmos](www.desmos.com/calculator), you can type the test statistic formula directly, replacing the values with those from your problem:

$$z = \frac{106.3 - 100}{15/\sqrt{40}}$$

Desmos will calculate the result immediately. Compare this value to your critical value (found using the same method described in Lesson 18.1) to make your decision.
