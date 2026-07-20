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
<title>Solution for practice 15.3.2</title>
</head>

## 15.3 Probability from a Normal Distribution - Solution for Practice 2
2. Using the same tire data ($\mu = 50{,}000$ miles, $\sigma = 4{,}000$ miles), find the probability that a randomly selected tire lasts **more than 58,000 miles**.

### Solution

**Step 1: Find the z-score.**

$$z=\frac{58{,}000-50{,}000}{4{,}000}=\frac{8{,}000}{4{,}000}=2.00$$

**Step 2: Find the area to the LEFT of $z=2.00$, then subtract from 1 to get the area to the right.**

$$P(z<2.00)=0.9772$$

$$P(z>2.00)=1-0.9772=0.0228$$

The probability that a randomly selected tire lasts more than 58,000 miles is about **0.0228, or 2.28%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson15/15_3_ProbabilityFromNormal.html#practice)
