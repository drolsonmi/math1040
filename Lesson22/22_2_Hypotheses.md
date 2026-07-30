<head>
<title>22.2 Hypotheses of 2 Independent Samples</title>
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

# Lesson 22.2 Hypotheses of 2 Independent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.2 Setting up hypotheses for a difference of means (pages 210-211)

## Lesson
When we compared a single sample to a claimed value, our null hypothesis was $H_0: \mu = \mu_0$. Now that we have **two** independent samples, we no longer have a claimed value to compare to — instead, we compare the two population means, $\mu_1$ and $\mu_2$, directly to each other.

### The Null and Alternate Hypotheses
Our default assumption is that there is **no difference** between the two population means:

$$H_0: \mu_1 = \mu_2 \qquad \text{(equivalently, } \mu_1 - \mu_2 = 0\text{)}$$

The alternate hypothesis again takes one of three forms:

| Research Question                      | Alternate Hypothesis   | Test Type    |
| :------------------------------------- | :--------------------: | :----------- |
| Is $\mu_1$ **greater than** $\mu_2$?   | $H_A: \mu_1 > \mu_2$   | Right-tailed |
| Is $\mu_1$ **less than** $\mu_2$?      | $H_A: \mu_1 < \mu_2$   | Left-tailed  |
| Is $\mu_1$ **different from** $\mu_2$? | $H_A: \mu_1 \ne \mu_2$ | Two-tailed   |

It doesn't matter which group you call "Group 1" and which you call "Group 2" — just be consistent throughout the problem, and make sure your conclusion reflects your choice.

### Verifying the Conditions
Before comparing two means, we need to verify:
1. **Both samples are random**
2. **The two samples are independent of each other** (see Lesson 22.1)
3. **Each sample is large enough.** For each group, either the sample size is at least 30 ($n_1 \ge 30$ and $n_2 \ge 30$), or the population it comes from is normally distributed.

If all three conditions hold, we can model the difference in sample means, $\bar{x}_1 - \bar{x}_2$, using a t-distribution.

### Example

> A city wants to know whether the average customer wait time is different between its two coffee shop locations. A random sample of 32 customers at Location A had an average wait time of 4.8 minutes with a standard deviation of 1.1 minutes. An independent random sample of 35 customers at Location B had an average wait time of 4.3 minutes with a standard deviation of 0.9 minutes. Test at the 5% significance level.

**Identifying the information:**
* Location A: $n_1 = 32$, $\bar{x}_1 = 4.8$, $s_1 = 1.1$
* Location B: $n_2 = 35$, $\bar{x}_2 = 4.3$, $s_2 = 0.9$

**Setting up the hypotheses:**

We are testing whether the two wait times are simply **different**, with no direction specified:

$$H_0: \mu_1 = \mu_2 \qquad\qquad H_A: \mu_1 \ne \mu_2 \quad \text{(two-tailed)}$$

**Verifying the conditions:**
* Both samples are random — *stated in the problem*
* The two samples are independent — *different customers at two different locations*
* Both samples are large enough: $n_1 = 32 \ge 30$ ✓ and $n_2 = 35 \ge 30$ ✓

All conditions are satisfied, so we can proceed with a hypothesis test in Lesson 22.4.

## Practice
For each of the following questions, identify the two sample statistics, state both hypotheses, and verify the conditions of the central limit theorem are satisfied.

1. An education researcher wants to know if there is a difference in average test scores between School A and School B. A random sample of 40 students at School A had an average score of 78.4 with a standard deviation of 8.2. An independent random sample of 38 students at School B had an average score of 74.9 with a standard deviation of 7.5. Test at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/22_2_Solution1.md)
2. A fitness researcher wants to know if Program X leads to greater average weight loss than Program Y. A random sample of 25 participants using Program X lost an average of 12.3 lbs with a standard deviation of 3.1 lbs. An independent random sample of 28 participants using Program Y lost an average of 9.8 lbs with a standard deviation of 2.8 lbs. Test at the 1% significance level.
    * [After solving on your own, see solution here](Solutions/22_2_Solution2.md)
3. A transit planner wants to know if Bus Route 1 has a shorter average travel time than Bus Route 2. A random sample of 30 trips on Route 1 averaged 22.5 minutes with a standard deviation of 4.0 minutes. An independent random sample of 32 trips on Route 2 averaged 25.1 minutes with a standard deviation of 4.6 minutes. Test at the 5% significance level.
    * [After solving on your own, see solution here](Solutions/22_2_Solution3.md)
