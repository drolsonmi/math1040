<head>
<title>20.5 Hypothesis Testing with 1 Quantitative Sample</title>
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

# Lesson 20.5 Hypothesis Testing with 1 Quantitative Sample
## Reading

## Lesson
We've now covered every piece of a hypothesis test: hypotheses, critical regions, test statistics, and p-values. In this lesson, we put it all together into a single, complete process, and use it to solve a problem from start to finish.

To carry out a hypothesis test for a mean, follow these steps:
1. Verify the Central Limit Theorem applies (if it doesn't, we can't continue)
2. Define the null and alternate hypotheses
3. Choose the level of significance and find the critical region (and/or find the p-value)
4. Calculate the test statistic
5. Make a decision and interpret the result

Let's work through a new example and see the process from top to bottom:

> A car dealership advertises that its most popular model gets an average of 32 miles per gallon (mpg) on the highway. A random sample of 40 cars of this model recorded an average of 30.8 mpg with a standard deviation of 3.1 mpg. At the 5% significance level, test the claim that the true average highway mileage is *less than* advertised.

### 1. Central Limit Theorem
* The sample is random — *this is satisfied*
* The sample is large enough ($n = 40 > 30$) — *this is satisfied*

Both conditions are satisfied, so we may continue.

### 2. Hypotheses
The claim is that the gas mileage of this popular car model gets an average gas mileage of 32 mpg, so our null value is $\mu_0 = 32$. We are testing to see if the gas mileage is less than 32 mpg. That means we are doing a two-tailed test:

$$H_0: \mu = 32 \qquad\qquad H_A: \mu < 32$$

### 3. Level of Significance and Critical Region
We are given $\alpha = 0.05$. Since we do not know the population standard deviation ($\sigma$), we will use the t-distribution, with degrees of freedom $df = n - 1 = 39$.

Since this is a left-tailed test, the critical value is going to be negative. For a left-tailed test at $\alpha = 0.05$ with $df = 39$, the critical value is,

$$t_c \approx -1.685$$

so the critical region is $t  < -1.685$.

### 4. Test Statistic
Since we only have the sample standard deviation ($s = 3.1$), we use a t-score:

$$t = \frac{\bar{x}-\mu_0}{s/\sqrt{n}} = \frac{30.8-32}{3.1/\sqrt{40}} = \frac{-1.2}{0.4902} \approx -2.448$$

We can also find the p-value for this test statistic. The t-score we just calculated is negative, so that means we are in the left tail. Using a calculator,

$$p = P(T < -2.448) \approx 0.0095$$

### 5. Decision and Interpretation
Option 1:
- Using the critical region: our test statistic, $t \approx -2.448$, falls inside the critical region ($t < -1.685$), so we __reject the null hypothesis__.

Option 2:
- Using the p-value: $p \approx 0.0095$ is less than the level of significance $\alpha = 0.05$, so we again __reject the null hypothesis__.

Both approaches give the same result, as they always will. The null hypothesis is that the gas mileage is around 32 mpg. Since this is rejected, we adopt our alternate hypothesis that the true average gas mileage is less than that. Our conclusion:

> There is enough evidence, at the 5% significance level, to conclude that the average gas mileage for this popular car model is less than 32 mpg.


## Practice
For each of the following questions (same questions as in 20.2 and 20.3), state the correct hypotheses and determine the level of significance. Then use the p-value to make your decision and confirm that you reach the same conclusion as you did in 20.3.

1. A coffee shop claims that the average wait time for a customer to receive their order is no more than 4 minutes. A customer advocacy group believes the wait time is longer. A random sample of 35 customers had an average wait time of 4.6 minutes with a standard deviation of 1.2 minutes. At the 5% significance level, use the critical region method to test the claim.
    * [After solving on your own, see solution here](./Solutions/20_5_Solution1.md)
2. A smartphone manufacturer advertises that their new model has an average battery life of 20 hours. A tech reviewer suspects the battery life is less than advertised. A random sample of 55 phones showed an average battery life of 18.7 hours with a standard deviation of 2.5 hours. Conduct a hypothesis test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/20_5_Solution2.md)
3. An educator wants to test whether a new teaching method affects student performance. Historically, the average score on a standardized exam is 75. A random sample of 40 students taught with the new method had an average score of 78.2 with a standard deviation of 6.3. Test the hypothesis at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/20_5_Solution3.md)


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
