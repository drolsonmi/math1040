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

1. A researcher tests whether caffeine improves reaction time (in milliseconds). Reaction time is measured for 5 participants before and after drinking a cup of coffee. Find $\bar{d}$ and $s_d$ using $d = \text{Before} - \text{After}$.

## Solution

**Differences ($d = \text{Before} - \text{After}$):**

| Participant | Before | After | $d$ |
|---|---|---|---|
| 1 | 320 | 290 | 30 |
| 2 | 305 | 295 | 10 |
| 3 | 310 | 300 | 10 |
| 4 | 298 | 285 | 13 |
| 5 | 315 | 292 | 23 |

**Finding $\bar{d}$:**

\[\bar{d} = \frac{30+10+10+13+23}{5} = \frac{86}{5} = 17.2\]

**Finding $s_d$:**

| $d$ | $d-\bar{d}$ | $(d-\bar{d})^2$ |
|---|---|---|
| 30 | 12.8 | 163.84 |
| 10 | -7.2 | 51.84 |
| 10 | -7.2 | 51.84 |
| 13 | -4.2 | 17.64 |
| 23 | 5.8 | 33.64 |

\[\sum(d-\bar{d})^2 = 318.8 \qquad\qquad s_d = \sqrt{\frac{318.8}{4}} \approx 8.928\]

**Result:** $\bar{d} \approx 17.2$ ms, $s_d \approx 8.928$ ms, $n = 5$.

[Return back to Lesson 24.1](https://drolsonmi.github.io/math1040/Lesson24/24_1_DifferenceVariable.html#practice)
