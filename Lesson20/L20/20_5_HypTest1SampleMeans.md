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

# Lesson 20.5 Hypothesis Testing with 1 Sample (Means)
## Reading

## Lesson
We've now covered every piece of a hypothesis test: hypotheses, critical regions, test statistics, and p-values. In this lesson, we put it all together into a single, complete process, and use it to solve a problem from start to finish.

To carry out a hypothesis test for a mean, follow these steps:
1. Verify the Central Limit Theorem applies (if it doesn't, we can't continue)
2. Define the null and alternate hypotheses
3. Choose the level of significance and find the critical region (and/or find the p-value)
4. Calculate the test statistic
5. Make a decision and interpret the result

Let's work through the coffee shop example from Lessons 20.1 and 20.2:

> A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, test the claim that the average wait time is greater than 4 minutes.

#### 1. Central Limit Theorem
* The sample is random — *this is satisfied*
* The sample is large enough ($$n = 35 > 30$$) — *this is satisfied*

Both conditions are satisfied, so we may continue.

#### 2. Hypotheses
The claim is that the wait time is no more than 4 minutes, so our null value is $$\mu_0 = 4$$. The advocacy group believes the true wait time is *longer*, so this is a right-tailed test:

$$H_0: \mu = 4 \qquad\qquad H_A: \mu > 4$$

#### 3. Level of Significance and Critical Region
We are given $$\alpha = 0.05$$. Since we do not know the population standard deviation ($$\sigma$$), we will use the t-distribution, with degrees of freedom $$df = n - 1 = 34$$.

For a right-tailed test at $$\alpha = 0.05$$ with $$df = 34$$, the critical value is

$$t_c \approx 1.691$$

so the critical region is $$t > 1.691$$.

#### 4. Test Statistic
Since we only have the sample standard deviation ($$s = 1.2$$), we use a t-score:

$$t = \frac{\bar{x}-\mu_0}{s/\sqrt{n}} = \frac{4.6-4}{1.2/\sqrt{35}} = \frac{0.6}{0.2028} \approx 2.959$$

We can also find the p-value for this test statistic. This is a right-tailed test, so:

$$p = P(T > 2.959) \approx 0.0028$$

#### 5. Decision and Interpretation
Using the critical region: our test statistic, $$t \approx 2.959$$, falls inside the critical region ($$t > 1.691$$), so we __reject the null hypothesis__.

Using the p-value: $$p \approx 0.0028$$ is less than $$\alpha = 0.05$$, so we again __reject the null hypothesis__.

Both approaches agree, as they always will. Our conclusion:

> There is enough evidence, at the 5% significance level, to conclude that the average wait time for customers to receive their order is greater than 4 minutes.

This is also the exact same conclusion we reached in Lesson 20.2 using a confidence interval — the sample data are simply too far from the claimed value of 4 minutes for the null hypothesis to hold up, no matter which of the three methods (confidence interval, critical region, or p-value) we use to check it.

## Practice
1. A car dealership advertises that its most popular model gets an average of 32 miles per gallon (mpg) on the highway. A random sample of 40 cars of this model recorded an average of 30.8 mpg with a standard deviation of 3.1 mpg. At the 5% significance level, test the claim that the true average highway mileage is *less than* advertised.
    * After solving on your own, check the solution: <button popovertarget="Problem_1">Solution</button>
2. A university claims the average class size across campus is 28 students. A faculty senate member believes this has changed. A random sample of 45 classes shows an average size of 26.1 students with a standard deviation of 5.4 students. At the 1% significance level, test whether the true average class size is *different* from 28.
    * After solving on your own, see solution here <button popovertarget="Problem_2">Solution</button>
3. A fitness app claims users burn an average of 450 calories per workout session. The app developers want to know if a new workout plan increases this. A random sample of 32 sessions using the new plan shows an average of 468 calories burned with a standard deviation of 40 calories. At the 5% significance level, test whether the true average calories burned is *greater than* 450.
    * After solving on your own, see solution here <button popovertarget="Problem_3">Solution</button>

<div popover id="Problem_1">

## Problem 20.5.1
A car dealership advertises that its most popular model gets an average of __32 mpg__ on the highway. A __random sample of 40 cars__ recorded an average of __30.8 mpg__ with a __standard deviation of 3.1 mpg__. At the __5% significance level__, test the claim that the true average highway mileage is *less than* advertised.

__1. Central Limit Theorem__
* The sample is random
* The sample is large enough ($$n = 40 > 30$$)

Both conditions are satisfied.

__2. Hypotheses__

We are testing whether the true average is *less than* 32 mpg, so this is a left-tailed test:

$$H_0: \mu = 32 \qquad\qquad H_A: \mu < 32$$

__3. Level of Significance and Critical Region__

We don't know $$\sigma$$, so we use a t-distribution with $$df = 40 - 1 = 39$$. For $$\alpha = 0.05$$, left-tailed:

$$t_c \approx -1.685$$

The critical region is $$t < -1.685$$.

__4. Test Statistic__

$$t = \frac{30.8 - 32}{3.1/\sqrt{40}} = \frac{-1.2}{0.490} \approx -2.449$$

The p-value for this left-tailed test is

$$p = P(T < -2.449) \approx 0.0095$$

__5. Decision and Interpretation__

Since $$t \approx -2.449$$ falls inside the critical region ($$t < -1.685$$), and $$p \approx 0.0095 < \alpha = 0.05$$, we __reject the null hypothesis__.

There is enough evidence, at the 5% significance level, to conclude that the true average highway mileage is less than 32 mpg.

<center><button popovertarget="Problem_1" popovertargetaction="hide">Close</button></center>
</div>

<div popover id="Problem_2">

## Problem 20.5.2
A university claims the average class size across campus is __28 students__. A __random sample of 45 classes__ shows an average size of __26.1 students__ with a __standard deviation of 5.4 students__. At the __1% significance level__, test whether the true average class size is *different* from 28.

__1. Central Limit Theorem__
* The sample is random
* The sample is large enough ($$n = 45 > 30$$)

Both conditions are satisfied.

__2. Hypotheses__

We are testing whether the true average is *different* from 28, so this is a two-tailed test:

$$H_0: \mu = 28 \qquad\qquad H_A: \mu \ne 28$$

__3. Level of Significance and Critical Region__

We don't know $$\sigma$$, so we use a t-distribution with $$df = 45 - 1 = 44$$. For $$\alpha = 0.01$$, two-tailed ($$\alpha/2 = 0.005$$ in each tail):

$$t_c \approx \pm 2.692$$

The critical region is $$t < -2.692 \text{ or } t > 2.692$$.

__4. Test Statistic__

$$t = \frac{26.1 - 28}{5.4/\sqrt{45}} = \frac{-1.9}{0.805} \approx -2.360$$

The p-value for this two-tailed test is

$$p = 2 \times P(T > 2.360) \approx 2 \times 0.0113 = 0.0226$$

__5. Decision and Interpretation__

Since $$t \approx -2.360$$ does *not* fall inside the critical region ($$t < -2.692$$ or $$t > 2.692$$), and $$p \approx 0.0226 > \alpha = 0.01$$, we __fail to reject the null hypothesis__.

There is not enough evidence, at the 1% significance level, to conclude that the true average class size is different from 28 students.

<center><button popovertarget="Problem_2" popovertargetaction="hide">Close</button></center>
</div>
<div popover id="Problem_3">

## Problem 20.5.3
A fitness app claims users burn an average of __450 calories__ per workout session. A __random sample of 32 sessions__ using a new workout plan shows an average of __468 calories__ burned with a __standard deviation of 40 calories__. At the __5% significance level__, test whether the true average calories burned is *greater than* 450.

__1. Central Limit Theorem__
* The sample is random
* The sample is large enough ($$n = 32 > 30$$)

Both conditions are satisfied.

__2. Hypotheses__

We are testing whether the true average is *greater than* 450 calories, so this is a right-tailed test:

$$H_0: \mu = 450 \qquad\qquad H_A: \mu > 450$$

__3. Level of Significance and Critical Region__

We don't know $$\sigma$$, so we use a t-distribution with $$df = 32 - 1 = 31$$. For $$\alpha = 0.05$$, right-tailed:

$$t_c \approx 1.696$$

The critical region is $$t > 1.696$$.

__4. Test Statistic__

$$t = \frac{468 - 450}{40/\sqrt{32}} = \frac{18}{7.071} \approx 2.546$$

The p-value for this right-tailed test is

$$p = P(T > 2.546) \approx 0.0081$$

__5. Decision and Interpretation__

Since $$t \approx 2.546$$ falls inside the critical region ($$t > 1.696$$), and $$p \approx 0.0081 < \alpha = 0.05$$, we __reject the null hypothesis__.

There is enough evidence, at the 5% significance level, to conclude that the new workout plan increases the average calories burned above 450.

<center><button popovertarget="Problem_3" popovertargetaction="hide">Close</button></center>
</div>


## Technology

### TI-83/84
The TI-83/84 can run the whole test at once and give you the test statistic and p-value together:
* Press `STAT`
* Select the `TESTS` menu
* Select `1:Z-Test...` if $$\sigma$$ is known, or `2:T-Test...` if it is not
* Choose `Stats`, then enter $$\mu_0$$, $$\sigma$$ (or $$s_x$$), $$\bar{x}$$, and $$n$$
* Choose the alternate hypothesis (`$$\ne \mu_0$$`, `$$<\mu_0$$`, or `$$>\mu_0$$`)
* Select "Calculate"

The calculator returns the test statistic (`z` or `t`) and the p-value. Compare the p-value to $$\alpha$$ (or the test statistic to your critical value) to make your decision.

### Excel
Build the test statistic and p-value from their pieces, just as in Lessons 20.3 and 20.4.

__Test Statistic:__
* Type `=(` followed by the cell with $$\bar{x}$$, `-`, the cell with $$\mu_0$$, `)/(`, the cell with $$s$$ (or $$\sigma$$), `/SQRT(`, the cell with $$n$$, `))`
  * For example: `=(B1-B2)/(B3/SQRT(B4))`

__P-value (t-distribution, since $$\sigma$$ is usually unknown):__ use `T.DIST` for a left-tailed p-value, `1-T.DIST` for right-tailed, or `T.DIST.2T` for two-tailed.
* Right-tailed: `=1-T.DIST(t,df,TRUE)`
* Left-tailed: `=T.DIST(t,df,TRUE)`
* Two-tailed: `=T.DIST.2T(ABS(t),df)`

Replace `t` with the cell containing your test statistic and `df` with $$n-1$$.

### Desmos
In [Desmos](www.desmos.com/calculator), type the test statistic formula directly:

$$t = \frac{4.6 - 4}{1.2/\sqrt{35}}$$

Replace the values with those from your own problem. To find the critical value, follow the same method described in Lesson 18.5 for finding t critical values, using your level of significance ($$\alpha$$) in place of $$1-\text{confidence level}$$.
