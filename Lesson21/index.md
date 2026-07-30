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

## Lesson 21
### Outline
Lesson 20 covered hypothesis testing for quantitative data, where we tested a population mean ($\mu$) using z-scores or t-scores. This lesson applies the same reasoning to **categorical** data, where instead we test a population **proportion** ($p$).

* **21.1** sets up the test: identifying the null value ($p_0$), writing the null and alternate hypotheses, and verifying that the Central Limit Theorem applies to a proportion (the success-failure condition in place of $n \ge 30$).
* **21.2** covers the calculations: finding the standard error and test statistic (always a z-score for proportions), and using it to find the critical value and/or the p-value.
* **21.3** combines everything into the same five-step process used in Lesson 20.5 — CLT, hypotheses, test statistic, critical value/p-value, and conclusion — applied from start to finish to a full proportion problem.

By the end of the lesson, you'll be able to run a complete hypothesis test for a proportion, by hand, on a calculator, in Excel, or in Desmos, and correctly interpret the result in the context of the original question.

### Outcomes
By the end of this lesson, you should be able to:
* Identify the null value ($p_0$) and sample proportion ($\hat{p}$) from a categorical research question
* Write the null and alternate hypotheses for a test of a single proportion, and identify the test as left-tailed, right-tailed, or two-tailed
* Verify that the Central Limit Theorem applies to a proportion, using the random sample, success-failure, and independence conditions
* Calculate the standard error and test statistic (z-score) for a single proportion
* Find the critical value and/or p-value for a proportion test, and use either to make a decision
* Carry out a complete hypothesis test for a single proportion, from hypotheses to a plain-language conclusion
* Perform each of these calculations using a TI-83/84 calculator, Excel, and Desmos

### Topics in this lesson
* [21.1 Categorical Hypotheses](./21_1_CatHypotheses.md)
* [21.2 Critical Values and P-Values](./21_2_CatCriticalAndP.md)
* [21.3 Full Categorical Hypothesis Test](./21_3_FullCatHypTests.md)
