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

## Practice
1. A pharmaceutical company claims that 70% of patients who take their medication experience significant improvement. A research group suspects the true rate is lower. In a clinical trial with a random sample of 150 patients, 96 experienced significant improvement. At the 5% significance level, find the test statistic and the p-value.

## Solution
From Lesson 21.1 we have:
* $p_0 = 0.70$, $n = 150$, $x = 96$, $\hat{p} = 0.64$
* $H_0: p = 0.70 \qquad H_A: p < 0.70$ (left-tailed)
* CLT verified ✓

**Standard Error:**

$$SE = \sqrt{\frac{p_0(1-p_0)}{n}} = \sqrt{\frac{0.70(0.30)}{150}} = \sqrt{\frac{0.21}{150}} = \sqrt{0.0014} = 0.03742$$

**Test Statistic:**

$$z = \frac{\hat{p} - p_0}{SE} = \frac{0.64 - 0.70}{0.03742} = \frac{-0.06}{0.03742} = -1.603$$

**Critical Value** (left-tailed, $\alpha = 0.05$): $z_c = -1.645$

**P-value** (left-tailed):

$$p = P(Z < -1.603)$$

On TI-84: `normalcdf(-1E99, -1.603, 0, 1)` $\approx 0.0545$

**Decision:**
* Critical region: $z = -1.603 > z_c = -1.645$ → Test statistic does **not** fall in the critical region
* P-value: $p = 0.0545 > \alpha = 0.05$ → **Fail to reject $H_0$**

**Conclusion:** There is **not** sufficient evidence at the 5% significance level to conclude that the true improvement rate is lower than 70%.

[Return back to Lesson 21.2](../21_2_CatCriticalAndP.md#practice)
