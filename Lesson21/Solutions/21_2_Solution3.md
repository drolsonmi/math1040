<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice
3. A city council claims that 60% of residents approve of a new park development plan. An opposition group believes the approval rate is lower. A random survey of 180 residents finds that 99 approve. At the 5% significance level, find the test statistic and the p-value.

## Solution
From Lesson 21.1 we have:
* $$p_0 = 0.60$$, $$n = 180$$, $$x = 99$$, $$\hat{p} = 99/180 \approx 0.55$$
* $$H_0: p = 0.60 \qquad H_A: p < 0.60$$ (left-tailed)
* CLT verified ✓

**Standard Error:**

$$SE = \sqrt{\frac{p_0(1-p_0)}{n}} = \sqrt{\frac{0.60(0.40)}{180}} = \sqrt{\frac{0.24}{180}} = \sqrt{0.001\overline{3}} = 0.03651$$

**Test Statistic:**

$$z = \frac{\hat{p} - p_0}{SE} = \frac{0.55 - 0.60}{0.03651} = \frac{-0.05}{0.03651} = -1.370$$

**Critical Value** (left-tailed, $$\alpha = 0.05$$): $$z_c = -1.645$$

**P-value** (left-tailed):

$$p = P(Z < -1.370)$$

On TI-84: `normalcdf(-1E99, -1.370, 0, 1)` $$\approx 0.0853$$

**Decision:**
* Critical region: $$z = -1.370 > z_c = -1.645$$ → Test statistic does **not** fall in the critical region
* P-value: $$p = 0.0853 > \alpha = 0.05$$ → **Fail to reject $$H_0$$**

**Conclusion:** There is **not** sufficient evidence at the 5% significance level to conclude that fewer than 60% of residents approve of the park development plan.

[Return back to Lesson 21.2](../21_2_CatCriticalAndP.md#practice)
