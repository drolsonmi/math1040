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
<title>Solution for practice 15.4.3</title>
</head>

## 15.4 Finding Z-scores from a Probability - Solution for Practice 3
3. Pizza delivery times are approximately normally distributed with $\mu = 45$ minutes and $\sigma = 5$ minutes. Find the two delivery times that bound the **middle 90%** of all deliveries.

### Solution

**Step 1: Find the z-scores that bound the middle 90%.**

If the middle 90% is bounded, then $100\% - 90\% = 10\%$ is split evenly between the two tails, or 5% in each tail. This means we need the z-scores with 0.05 area to the left and 0.95 area to the left:

$$z=\pm 1.645$$

**Step 2: Convert each z-score to a data value.**

$$x_{\text{low}}=45+(-1.645)(5)=45-8.225\approx 36.78$$

$$x_{\text{high}}=45+(1.645)(5)=45+8.225\approx 53.23$$

The middle 90% of delivery times fall between about **36.78 minutes and 53.23 minutes**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson15/15_4_FindingZScore.html#practice)
