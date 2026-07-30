<head>
<title>25.1 Hypotheses for a Correlation Test</title>
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

# Lesson 25.1 Hypotheses for a Correlation Test
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 7.1.4 Testing for a linear relationship (pages 275-278)

## Lesson
Back when we studied correlation, we calculated $$r$$, the **sample** correlation coefficient, to measure the strength and direction of a linear relationship between two quantitative variables. But just like a sample mean ($$\bar{x}$$) or sample proportion ($$\hat{p}$$), $$r$$ is only an estimate. The true, population-level correlation is denoted $$\rho$$ (the Greek letter "rho").

A correlation hypothesis test asks: is the relationship we see in our sample ($$r$$) strong enough to conclude there's a real linear relationship in the population ($$\rho \ne 0$$), or could it just be due to random sampling variation?

#### The Null and Alternate Hypotheses
Our default assumption is that there is **no linear relationship** in the population:

$$H_0: \rho = 0$$

The alternate hypothesis takes one of the same three familiar forms:

| Research Question | Alternate Hypothesis | Test Type |
|---|---|---|
| Is there a **positive** linear relationship? | $$H_A: \rho > 0$$ | Right-tailed |
| Is there a **negative** linear relationship? | $$H_A: \rho < 0$$ | Left-tailed |
| Is there a linear relationship **at all**? | $$H_A: \rho \ne 0$$ | Two-tailed |

#### Verifying the Conditions
Before testing a correlation, we should check:
1. **The sample is random**
2. **The relationship looks linear.** A scatterplot of the data should show a roughly straight-line pattern — correlation only measures *linear* association, so a strong curved relationship can still produce a small, misleading $$r$$.
3. **No extreme outliers.** A single unusual point can drastically inflate or deflate $$r$$.

We'll take these conditions at face value in this course, based on the description of the study and a look at the scatterplot — a full check of the underlying distributional assumptions is beyond what we'll need here.

#### Example

> A teacher wants to know if there's a relationship between hours spent studying and exam scores. A random sample of 25 students shows a sample correlation of $$r = 0.52$$ between study hours and exam score. Is there evidence of a positive linear relationship? Test at the 5% significance level.

**Setting up the hypotheses:**

We are testing whether the relationship is **positive**:

$$H_0: \rho = 0 \qquad\qquad H_A: \rho > 0 \quad \text{(right-tailed)}$$

**Verifying the conditions:**
* The sample is random — *stated in the problem*
* We'll assume the scatterplot of study hours vs. exam scores shows a reasonably linear pattern with no extreme outliers

With the conditions satisfied, we're ready to test this correlation in Lesson 25.2.

## Practice
For each of the following, state both hypotheses and identify the test type.

1. A business analyst wants to know if there's a positive relationship between advertising spend and sales revenue. A random sample of 15 months shows a sample correlation of $$r = 0.68$$. Test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/25_1_Solution1.md)
2. A researcher wants to know if more screen time is associated with less sleep. A random sample of 20 teenagers shows a sample correlation of $$r = -0.45$$ between daily screen time and hours of sleep. Test at the 1% significance level.
    * [After solving on your own, see solution here](./Solutions/25_1_Solution2.md)
3. An economist wants to know if there is any linear relationship at all between daily temperature and ice cream sales. A random sample of 30 days shows a sample correlation of $$r = 0.39$$. Test at the 5% significance level.
    * [After solving on your own, see solution here](./Solutions/25_1_Solution3.md)
