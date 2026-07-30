<head>
<title>25.2 Testing the Correlation Coefficient</title>
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

# Lesson 25.2 Testing the Correlation Coefficient
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 7.1.4 Testing for a linear relationship (pages 275-278)

## Lesson
With the hypotheses from Lesson 25.1 in hand, testing a correlation follows the exact same five-step process we've used throughout this course. The only new piece is the test statistic itself — and in practice, you'll almost always let technology calculate it for you, so we won't dwell on the formula.

### The Test Statistic
$$t = \frac{r\sqrt{n-2}}{\sqrt{1-r^2}} \qquad\qquad df = n-2$$

Notice this uses a t-distribution, with $n-2$ degrees of freedom (we "use up" two degrees of freedom estimating the slope and intercept of the underlying relationship). Beyond that, the mechanics are identical to every other t-test we've done: find the test statistic, compare it to a critical value and/or p-value, and make a decision.

### The Five Steps

**Step 1 — Verify the Conditions:** random sample, roughly linear relationship, no extreme outliers (Lesson 25.1)

**Step 2 — State the Hypotheses:** $H_0: \rho = 0$, with $H_A$ matching the direction of the research question

**Step 3 — Compute the Test Statistic:** using the formula above (or, more commonly, technology)

**Step 4 — Find the Critical Value and/or P-Value:** exactly as with any other t-test

**Step 5 — Make a Decision and Write a Conclusion:** reject $H_0$ if the test statistic is in the critical region, or if $p\text{-value} \le \alpha$

### Example

> A teacher wants to know if there's a relationship between hours spent studying and exam scores. A random sample of 25 students shows a sample correlation of $r = 0.52$ between study hours and exam score. Is there evidence of a positive linear relationship? Test at the 5% significance level.

From Lesson 25.1: $H_0: \rho = 0$, $H_A: \rho > 0$ (right-tailed), conditions verified ✓.

**Test Statistic:**

$$t = \frac{0.52\sqrt{25-2}}{\sqrt{1-0.52^2}} = \frac{0.52\sqrt{23}}{\sqrt{0.7296}} = \frac{2.494}{0.854} \approx 2.919 \qquad df = 23$$

**Critical Value** (right-tailed, $\alpha = 0.05$, $df = 23$): $t_c \approx 1.714$

**P-value:** $p \approx 0.0038$

**Decision:** Since $t = 2.919 > t_c = 1.714$ (and $p \approx 0.0038 \le \alpha = 0.05$), we **reject $H_0$**.

**Conclusion:** There is sufficient evidence at the 5% significance level to conclude that there is a positive linear relationship between hours studied and exam scores.

## Practice
1. A business analyst wants to know if there's a positive relationship between advertising spend and sales revenue. A random sample of 15 months shows a sample correlation of $r = 0.68$. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/25_2_Solution1.md)
2. A researcher wants to know if more screen time is associated with less sleep. A random sample of 20 teenagers shows a sample correlation of $r = -0.45$ between daily screen time and hours of sleep. Conduct a full hypothesis test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/25_2_Solution2.md)
3. An economist wants to know if there is any linear relationship at all between daily temperature and ice cream sales. A random sample of 30 days shows a sample correlation of $r = 0.39$. Conduct a full hypothesis test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/25_2_Solution3.md)

## Technology
### TI-83/84
The TI-84 can run this entire test — including calculating $r$ from raw data — in one step.
* Enter your two lists of raw data in `L1` and `L2` (if you only have $r$ and $n$, see the note below)
* Make sure Diagnostics are turned on: `2ND` → `0` (Catalog) → scroll to `DiagnosticOn` → `Enter` → `Enter` (only needs to be done once)
* Press `STAT` → `[TESTS]` → `E:LinRegTTest...`
* Set `Xlist: L1`, `Ylist: L2`, `Freq: 1`
* Choose the direction of $H_A$ ($\ne 0$, $< 0$, or $> 0$)
* Leave `RegEQ` blank unless you want the regression equation stored
* Select `Calculate`

The output includes the test statistic (`t`), the p-value, the correlation ($r$), and $df$ — everything you need for Step 5.

> __Note:__ If you're only given summary values ($r$ and $n$, not raw data), you can still compute the test statistic directly using the formula above, then find the p-value with `tcdf(...)` just as you would for any other t-test.

### Excel
1. If you have raw data, find $r$ with `=CORREL(range1,range2)`
2. Find the test statistic: `=r*SQRT(n-2)/SQRT(1-r^2)`
3. Find the p-value using `T.DIST`:
    * Right-tailed: `=1-T.DIST(t,n-2,TRUE)`
    * Left-tailed: `=T.DIST(t,n-2,TRUE)`
    * Two-tailed: `=T.DIST.2T(ABS(t),n-2)`

### Desmos
In [Desmos](www.desmos.com/calculator), you can find $r$ directly from a data table using linear regression, or type the test statistic formula in if $r$ is already known:

$$t = \frac{0.52\sqrt{25-2}}{\sqrt{1-0.52^2}}$$

Replace the values with those from your own problem, and compare the result to a critical value found using the t-distribution method from Lesson 18.5.
