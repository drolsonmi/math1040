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
<title>Solution for practice 15.4.2</title>
</head>

## 15.4 Finding Z-scores from a Probability - Solution for Practice 2
2. Metal rod lengths are approximately normally distributed with $\mu = 5$ cm and $\sigma = 0.05$ cm. Find the length that separates the shortest **5%** of rods from the rest.

### Solution

**Step 1: Find the z-score with 0.05 area to its left.**

Since we want the *shortest* 5%, we need the z-score with only 5% of the area to its left, which is a negative z-score:

$$z\approx -1.645$$

**Step 2: Convert the z-score to a data value.**

$$x=\mu+z\cdot\sigma=5+(-1.645)(0.05)=5-0.08225\approx 4.92$$

A length of about **4.92 cm** separates the shortest 5% of rods from the rest.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson15/15_4_FindingZScore.html#practice)
