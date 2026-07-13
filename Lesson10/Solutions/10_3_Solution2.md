<head>
<title>Solution for practice 10.3.2</title>
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

## 10.3 Conditional Probabilities - Solution for Practice 2

1. Find $P(\text{has a job} \mid \text{no car})$, and compare it to $P(\text{job})$.

| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |

### Solution

Since we're told the student has no car, we restrict our attention to the "No Car" row (100 students), and ask how many of those 100 have a job (50):

$$P(\text{job} \mid \text{no car}) = \frac{50}{100} = 0.5$$

**Comparison**: The overall (unconditional) probability of having a job is:

$$P(\text{job}) = \frac{110}{200} = 0.55$$

Since $P(\text{job} \mid \text{no car}) = 0.5$ is different from $P(\text{job}) = 0.55$, knowing that a student doesn't own a car actually changes the probability that they have a job (it goes down slightly, from 55% to 50%). This is another sign that car ownership and having a job are **not independent** of each other — we'll formally test for independence in 10.5.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_3_ConditionalProbabilities.html#practice)
