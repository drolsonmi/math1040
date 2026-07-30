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

1. An instructor wants to know if a review session improves exam scores. 6 students take a pretest, attend the review session, then take a posttest. Find $\bar{d}$ and $s_d$ using $d = \text{Posttest} - \text{Pretest}$.

## Solution

**Differences ($d = \text{Posttest} - \text{Pretest}$):**

| Student | Pretest | Posttest | $d$ |
|---|---|---|---|
| 1 | 62 | 68 | 6 |
| 2 | 70 | 74 | 4 |
| 3 | 58 | 65 | 7 |
| 4 | 75 | 78 | 3 |
| 5 | 66 | 70 | 4 |
| 6 | 80 | 79 | -1 |

**Finding $\bar{d}$:**

\[\bar{d} = \frac{6+4+7+3+4+(-1)}{6} = \frac{23}{6} \approx 3.833\]

**Finding $s_d$:**

| $d$ | $d-\bar{d}$ | $(d-\bar{d})^2$ |
|---|---|---|
| 6 | 2.167 | 4.694 |
| 4 | 0.167 | 0.028 |
| 7 | 3.167 | 10.028 |
| 3 | -0.833 | 0.694 |
| 4 | 0.167 | 0.028 |
| -1 | -4.833 | 23.361 |

\[\sum(d-\bar{d})^2 \approx 38.833 \qquad\qquad s_d = \sqrt{\frac{38.833}{5}} \approx 2.787\]

**Result:** $\bar{d} \approx 3.833$ points, $s_d \approx 2.787$ points, $n = 6$.

[Return back to Lesson 24.1](https://drolsonmi.github.io/math1040/Lesson24/24_1_DifferenceVariable.html#practice)
