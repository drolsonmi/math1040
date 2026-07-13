<head>
<title>Solution for practice 10.3.1</title>
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

## 10.3 Conditional Probabilities - Solution for Practice 1

1. Find $P(\text{owns a car} \mid \text{no job})$.

| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |

### Solution

Since we're told the student has no job, we restrict our attention to the "No Job" **column** (90 students), and ask how many of those 90 also own a car (40):

$$P(\text{car} \mid \text{no job}) = \frac{40}{90} = \frac{4}{9} \approx 0.444$$

We get the same result using the formula directly:

$$P(\text{car} \mid \text{no job}) = \frac{P(\text{car and no job})}{P(\text{no job})} = \frac{40/200}{90/200} = \frac{0.2}{0.45} \approx 0.444$$

The probability that a student owns a car, given that they have no job, is approximately **0.444, or 44.4%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_3_ConditionalProbabilities.html#practice)
