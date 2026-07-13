<head>
<title>Solution for practice 10.1.2</title>
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

## 10.1 OR Probabilities - Solution for Practice 2

1. Using the survey table from the lesson (200 college students, car ownership vs. part-time job), find the probability that a randomly selected student **owns a car OR does not have a job**.

| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |

### Solution

**Step 1: Find each individual probability directly from the table.**

$$P(\text{car}) = \frac{100}{200} = 0.5, \qquad P(\text{no job}) = \frac{90}{200} = 0.45$$

**Step 2: Find the overlap** — students who own a car **and** have no job.

$$P(\text{car and no job}) = \frac{40}{200} = 0.2$$

**Step 3: Apply the general addition rule.**

$$P(\text{car or no job}) = P(\text{car}) + P(\text{no job}) - P(\text{car and no job}) = 0.5 + 0.45 - 0.2 = 0.75$$

The probability that a randomly selected student owns a car or does not have a job is **0.75, or 75%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_1_ORProbabilities.html#practice)
