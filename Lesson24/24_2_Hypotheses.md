<head>
<title>24.2 Hypotheses for Paired Data</title>
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

# Lesson 24.2 Hypotheses for Paired Data
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.1 Paired data (page 209)

## Lesson
Now that we know how to build the difference variable $d$ (Lesson 24.1), setting up hypotheses is nothing new — it's exactly Lesson 20.1, just applied to $d$ instead of $x$.

### The Null and Alternate Hypotheses
Since $H_0$ always claims there is no effect, the null value for a paired difference is always **0**:

$$H_0: \mu_d = 0$$

The alternate hypothesis takes one of the same three familiar forms:

| Research Question | Alternate Hypothesis | Test Type |
|---|---|---|
| Is the mean difference **greater than** 0? | $H_A: \mu_d > 0$ | Right-tailed |
| Is the mean difference **less than** 0? | $H_A: \mu_d < 0$ | Left-tailed |
| Is the mean difference **different from** 0? | $H_A: \mu_d \ne 0$ | Two-tailed |

> __Watch the direction of subtraction!__ If $d = x_1 - x_2$, then $\mu_d > 0$ means group 1 tends to be larger. But if you'd subtracted the other way ($d = x_2 - x_1$), that same conclusion would show up as $\mu_d < 0$ instead. Neither order is "wrong" — just be consistent, and make sure your hypotheses and your final conclusion match the order you chose in Lesson 24.1.

### Verifying the Conditions
Because this is really a one-sample t-test on $d$, the conditions are the same ones from Lesson 20.5, applied to the differences rather than the original data:
1. **The sample of pairs is random**
2. **The sample is large enough:** either $n \ge 30$, or the population of differences is approximately normally distributed

Notice that the condition is about the *differences* being large enough or normal — not the two original variables. Two skewed variables can easily produce a nicely symmetric set of differences, and vice versa, so always check the condition using $d$ itself.

### Example

> A clinic wants to know whether a new medication lowers systolic blood pressure. Blood pressure is measured for 10 patients before starting the medication, and again after 4 weeks on the medication. Test at the 5% significance level.

From Lesson 24.1: $\bar{d} = 6.5$, $s_d \approx 2.677$, $n = 10$, using $d = \text{Before} - \text{After}$.

**Setting up the hypotheses:**

If the medication works, we'd expect Before to be larger than After, so $d$ should tend to be **positive**. This is a right-tailed test:

$$H_0: \mu_d = 0 \qquad\qquad H_A: \mu_d > 0$$

**Verifying the conditions:**
* The sample of 10 patients is random — *stated in the problem*
* The sample size is small ($n = 10 < 30$), so we need the differences to be approximately normal. A quick check of the 10 differences (1, 3, 6, 7, 7, 7, 8, 8, 8, 10) shows a roughly symmetric, single-peaked spread with no extreme outliers, so we'll treat this condition as satisfied.

Both conditions are satisfied, so we can proceed with a hypothesis test in Lesson 24.4.

## Practice
For each of the following, state both hypotheses and verify the conditions, using the differences you calculated in Lesson 24.1.

1. A researcher tests whether caffeine improves (lowers) reaction time. Reaction time was measured for 5 participants before and after drinking a cup of coffee, using $d = \text{Before} - \text{After}$ (from Lesson 24.1: $\bar{d} = 17.2$, $s_d \approx 8.928$, $n = 5$). Test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/24_2_Solution1.md)
2. An instructor wants to know if a review session improves (raises) exam scores. Scores were measured for 6 students before and after the session, using $d = \text{Posttest} - \text{Pretest}$ (from Lesson 24.1: $\bar{d} \approx 3.833$, $s_d \approx 2.787$, $n = 6$). Test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/24_2_Solution2.md)
3. A nutritionist wants to know if a 6-week diet program changes participants' weight. Weight was measured for 5 participants before and after the program, using $d = \text{Before} - \text{After}$ (from Lesson 24.1: $\bar{d} = 6.6$, $s_d \approx 1.517$, $n = 5$). Test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/24_2_Solution3.md)
