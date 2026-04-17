<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
2. A university reports that 30% of its students are first-generation college students. A student affairs office believes the proportion may be different from the reported value. They randomly survey 250 students and find that 85 are first-generation students. Test at the 10% significance level.

## Solution
**Identifying the information:**
* Null value: $$p_0 = 0.30$$
* Sample size: $$n = 250$$
* Number of successes: $$x = 85$$
* Sample proportion: $$\hat{p} = 85/250 = 0.34$$

**Hypotheses:**

The office believes the proportion may be **different** from 30% — either higher or lower.

$$H_0: p = 0.30 \qquad\qquad H_A: p \ne 0.30 \quad \text{(two-tailed)}$$

**Verify the Central Limit Theorem:**
* Random sample? **Yes** (stated in the problem)
* Success-failure condition:
  * $$np_0 = 250(0.30) = 75 \ge 10$$ ✓
  * $$n(1-p_0) = 250(0.70) = 175 \ge 10$$ ✓
* Independence: A university has far more than $$250 \times 10 = 2{,}500$$ students ✓

The Central Limit Theorem holds. We can proceed with the hypothesis test.

[Return back to Lesson 21.1](../21_1_CatHypotheses.md#practice)
