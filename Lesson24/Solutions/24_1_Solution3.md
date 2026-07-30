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

1. A nutritionist tracks the weight (in lbs) of 5 participants before and after a 6-week diet program. Find $\bar{d}$ and $s_d$ using $d = \text{Before} - \text{After}$.

## Solution

**Differences ($d = \text{Before} - \text{After}$):**

| Participant | Before | After | $d$ |
|---|---|---|---|
| 1 | 210 | 202 | 8 |
| 2 | 185 | 180 | 5 |
| 3 | 232 | 225 | 7 |
| 4 | 198 | 190 | 8 |
| 5 | 205 | 200 | 5 |

**Finding $\bar{d}$:**

\[\bar{d} = \frac{8+5+7+8+5}{5} = \frac{33}{5} = 6.6\]

**Finding $s_d$:**

| $d$ | $d-\bar{d}$ | $(d-\bar{d})^2$ |
|---|---|---|
| 8 | 1.4 | 1.96 |
| 5 | -1.6 | 2.56 |
| 7 | 0.4 | 0.16 |
| 8 | 1.4 | 1.96 |
| 5 | -1.6 | 2.56 |

\[\sum(d-\bar{d})^2 = 9.2 \qquad\qquad s_d = \sqrt{\frac{9.2}{4}} \approx 1.517\]

**Result:** $\bar{d} = 6.6$ lbs, $s_d \approx 1.517$ lbs, $n = 5$.

[Return back to Lesson 24.1](https://drolsonmi.github.io/math1040/Lesson24/24_1_DifferenceVariable.html#practice)
