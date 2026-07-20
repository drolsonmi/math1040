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
<title>Solution for practice 15.3.3</title>
</head>

## 15.3 Probability from a Normal Distribution - Solution for Practice 3
3. Package weights are approximately normally distributed with $\mu = 50$ lbs and $\sigma = 3$ lbs. Find the probability that a randomly selected package weighs **between 45 and 53 lbs**.

### Solution

**Step 1: Find the z-score for each boundary.**

$$z_a=\frac{45-50}{3}=\frac{-5}{3}\approx -1.67 \qquad z_b=\frac{53-50}{3}=\frac{3}{3}=1.00$$

**Step 2: Find the area to the left of each z-score.**

$$P(z<1.00)=0.8413 \qquad P(z<-1.67)=0.0475$$

**Step 3: Subtract the smaller area from the larger area to get the middle area.**

$$P(-1.67<z<1.00)=0.8413-0.0475=0.7938$$

The probability that a randomly selected package weighs between 45 and 53 lbs is about **0.7938, or 79.38%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson15/15_3_ProbabilityFromNormal.html#practice)
