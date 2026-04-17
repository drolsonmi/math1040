<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
3. A city council claims that 60% of residents approve of a new park development plan. An opposition group believes the approval rate is lower. A random survey of 180 residents finds that 99 approve. Conduct a full hypothesis test at the 5% significance level.

## Solution
From the problem:
* $$p_0 = 0.60$$, $$n = 180$$, $$x = 99$$, $$\hat{p} = 99/180 \approx 0.55$$
* $$\alpha = 0.05$$

**Step 1 — Verify the CLT**
* Random sample? **Yes**
* $$np_0 = 180(0.60) = 108 \ge 10$$ ✓ and $$n(1-p_0) = 180(0.40) = 72 \ge 10$$ ✓
* Independence: The city has far more than $$180 \times 10 = 1{,}800$$ residents ✓

**Step 2 — Hypotheses**

$$H_0: p = 0.60 \qquad\qquad H_A: p < 0.60 \quad \text{(left-tailed)}$$

**Step 3 — Test Statistic**

$$SE = \sqrt{\frac{0.60(0.40)}{180}} = \sqrt{0.001\overline{3}} = 0.03651$$

$$z = \frac{0.55 - 0.60}{0.03651} = \frac{-0.05}{0.03651} = -1.370$$

**Step 4 — Critical Value and P-Value**

* Critical value (left-tailed, $$\alpha = 0.05$$): $$z_c = -1.645$$
* P-value: `normalcdf(-1E99, -1.370, 0, 1)` $$\approx 0.0853$$

**Step 5 — Decision and Conclusion**

* $$z = -1.370 > z_c = -1.645$$ → Test statistic is **not** in the critical region
* $$p = 0.0853 > \alpha = 0.05$$ → **Fail to reject $$H_0$$**

**Conclusion:** There is **not** sufficient evidence at the 5% significance level to conclude that fewer than 60% of residents approve of the park development plan.

[Return back to Lesson 21.3](../21_3_FullCatHypTests.md#practice)
