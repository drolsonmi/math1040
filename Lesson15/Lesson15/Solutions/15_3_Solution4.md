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
<title>Solution for practice 15.3.4</title>
</head>

## 15.3 Probability from a Normal Distribution - Solution for Practice 4
4. Daily commute times are approximately normally distributed with $\mu = 32$ minutes and $\sigma = 6$ minutes. Find the probability that a randomly selected employee's commute is **between 20 and 44 minutes**, and compare your result to what the Empirical Rule would predict.

### Solution

**Step 1: Find the z-score for each boundary.**

$$z_a=\frac{20-32}{6}=\frac{-12}{6}=-2.00 \qquad z_b=\frac{44-32}{6}=\frac{12}{6}=2.00$$

**Step 2: Find the area to the left of each z-score.**

$$P(z<2.00)=0.9772 \qquad P(z<-2.00)=0.0228$$

**Step 3: Subtract to find the middle area.**

$$P(-2.00<z<2.00)=0.9772-0.0228=0.9544$$

The probability that a randomly selected employee's commute is between 20 and 44 minutes is about **0.9544, or 95.44%**.

Since 20 and 44 minutes are exactly 2 standard deviations below and above the mean, this matches almost exactly with the Empirical Rule, which estimates that about **95%** of values fall within 2 standard deviations of the mean. The Z-table simply gives us a more precise version of that same estimate.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson15/15_3_ProbabilityFromNormal.html#practice)
