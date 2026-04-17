<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
3. A city council claims that 60% of residents approve of a new park development plan. An opposition group believes the approval rate is lower. A random survey of 180 residents finds that 99 approve. Test at the 5% significance level.

## Solution
**Identifying the information:**
* Null value: $$p_0 = 0.60$$
* Sample size: $$n = 180$$
* Number of successes: $$x = 99$$
* Sample proportion: $$\hat{p} = 99/180 = 0.55$$

**Hypotheses:**

The opposition group believes the approval rate is **lower** than 60%.

$$H_0: p = 0.60 \qquad\qquad H_A: p < 0.60 \quad \text{(left-tailed)}$$

**Verify the Central Limit Theorem:**
* Random sample? **Yes** (stated in the problem)
* Success-failure condition:
  * $$np_0 = 180(0.60) = 108 \ge 10$$ ✓
  * $$n(1-p_0) = 180(0.40) = 72 \ge 10$$ ✓
* Independence: A city has far more than $$180 \times 10 = 1{,}800$$ residents ✓

The Central Limit Theorem holds. We can proceed with the hypothesis test.

[Return back to Lesson 21.1](../21_1_CatHypotheses.md#practice)
