<head>
<title>Solution for practice 10.4.1</title>
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

## 10.4 AND Probabilities - Solution for Practice 1

1. Using the survey table, we know $P(\text{no car}) = 0.5$ and $P(\text{no job} \mid \text{no car}) = 0.5$. Use the multiplication rule to find $P(\text{no car and no job})$, then check your answer against the table.

| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |

### Solution

**Apply the multiplication rule:**

$$P(\text{no car and no job}) = P(\text{no car}) \cdot P(\text{no job} \mid \text{no car}) = (0.5)(0.5) = 0.25$$

**Check against the table**: The number of students with no car and no job is 50, out of 200 total.

$$P(\text{no car and no job}) = \frac{50}{200} = 0.25$$

The two methods agree — the probability that a randomly selected student has no car and no job is **0.25, or 25%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_4_ANDProbabilities.html#practice)
