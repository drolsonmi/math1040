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
<title>Solution for practice 13.1.4</title>
</head>

## 13.1 What is a Binomial Distribution? - Solution for Practice 4
4. A teacher calls on students **one at a time, without replacement**, from a class of 25 students to answer questions until she has called on 5 students, and records how many of the 5 are wearing glasses.

### Solution

Check the four requirements:
- Fixed number of trials: yes, $n=5$ students are called on.
- Two outcomes: yes, each student either is wearing glasses (success) or is not (failure).
- Constant probability: **no**. Once a student is called on, they are removed from the pool, so the number of students wearing glasses left in the class (and therefore the probability for the next student) can change.
- Independent trials: **no**, for the same reason as above — the trials are linked because we are sampling without replacement.

Because the probability of success is not constant and the trials are not independent, this **is not a binomial experiment**. With a class of only 25 students and a sample of 5 (20% of the class), the population is not large enough for the "large population" approximation to be reasonable either.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_1_WhatIsBinomial.html#practice)
