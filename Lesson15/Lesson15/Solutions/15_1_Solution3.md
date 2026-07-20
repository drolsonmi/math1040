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
<title>Solution for practice 15.1.3</title>
</head>

## 15.1 Discrete and Continuous Distributions - Solution for Practice 3
3. Explain why it doesn't make sense to ask for the probability that a randomly selected adult weighs *exactly* 150 lbs, and describe how we would instead find a meaningful probability about that adult's weight.

### Solution

Weight is a **continuous** variable, meaning it can take on infinitely many possible values within any range (150 lbs, 150.1 lbs, 150.03 lbs, 150.028 lbs, and so on, forever). Since there are infinitely many possible values, no single exact value can claim any real share of the probability, so $P(X = 150) = 0$.

Instead, we find the probability that the adult's weight falls within an **interval**, such as between 148 and 152 lbs. For a continuous variable, this probability is represented by the **area under the density curve** between those two values.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson15/15_1_ContinuousVars.html#practice)
