<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
1. A pharmaceutical company claims that 70% of patients who take their medication experience significant improvement. A research group suspects the true rate is lower. In a clinical trial with a random sample of 150 patients, 96 experienced significant improvement. At the 5% significance level, test the company's claim.

## Solution
**Identifying the information:**
* Null value: $$p_0 = 0.70$$
* Sample size: $$n = 150$$
* Number of successes: $$x = 96$$
* Sample proportion: $$\hat{p} = 96/150 = 0.64$$

**Hypotheses:**

The research group suspects the true rate is **lower** than 70%.

$$H_0: p = 0.70 \qquad\qquad H_A: p < 0.70 \quad \text{(left-tailed)}$$

**Verify the Central Limit Theorem:**
* Random sample? **Yes** (stated in the problem)
* Success-failure condition:
  * $$np_0 = 150(0.70) = 105 \ge 10$$ ✓
  * $$n(1-p_0) = 150(0.30) = 45 \ge 10$$ ✓
* Independence: Clinical trial participants are drawn from a population much larger than $$150 \times 10 = 1{,}500$$ ✓

The Central Limit Theorem holds. We can proceed with the hypothesis test.

[Return back to Lesson 21.1](../21_1_CatHypotheses.md#practice)
