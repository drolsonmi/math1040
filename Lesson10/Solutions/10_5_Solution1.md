<head>
<title>Solution for practice 10.5.1</title>
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

## 10.5 Independent Events - Solution for Practice 1

1. Using the survey table, determine whether "owns a car" and "has a job" are independent events. Show your work by comparing $P(\text{car})$ to $P(\text{car} \mid \text{job})$.

| | Has a Job | No Job | Total |
| --- | --- | --- | --- |
| **Owns a Car** | 60 | 40 | 100 |
| **No Car** | 50 | 50 | 100 |
| **Total** | 110 | 90 | 200 |

### Solution

**Step 1: Find $P(\text{car})$**, the overall (unconditional) probability of owning a car.

$$P(\text{car}) = \frac{100}{200} = 0.5$$

**Step 2: Find $P(\text{car} \mid \text{job})$.** Restricting our attention to the 110 students who have a job, 60 of them own a car.

$$P(\text{car} \mid \text{job}) = \frac{60}{110} \approx 0.545$$

**Step 3: Compare the two values.**

$$P(\text{car}) = 0.5, \qquad P(\text{car} \mid \text{job}) \approx 0.545$$

Since $P(\text{car}) \ne P(\text{car} \mid \text{job})$, knowing that a student has a job **does** change the probability that they own a car. Therefore, **"owns a car" and "has a job" are dependent events, not independent**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson10/10_5_IndependentEvents.html#practice)
