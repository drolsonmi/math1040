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
<title>Solution for practice 8.4.3</title>
</head>

## 8.4 The Coefficient of Determination - Solution for Practice 3

1. A dataset has a coefficient of determination of $r^2 = 0.36$.
  - What percentage of the variation in $y$ is explained by the linear relationship with $x$?
  - What are the two possible values of the correlation coefficient $r$?
  - Can you tell from $r^2$ alone whether the relationship is positive or negative? Explain.

### Solution

**Percentage explained**: Since $r^2 = 0.36$, about **36%** of the variation in $y$ is explained by the linear relationship with $x$. The remaining 64% is due to other factors.

**Possible values of $r$**: Since $r^2 = 0.36$, we take the square root to find $r$:

$$r = \pm\sqrt{0.36} = \pm 0.6$$

So $r$ could be either $0.6$ or $-0.6$.

**Can we tell the direction from $r^2$ alone?** **No.** Since $r^2$ is found by squaring $r$, it loses all information about the sign. A coefficient of determination of $0.36$ is exactly the same whether the original relationship was $r = 0.6$ (a moderate-to-strong **positive** relationship) or $r = -0.6$ (a moderate-to-strong **negative** relationship). To determine the direction, we would need to know the sign of $r$ itself (or, equivalently, the sign of the slope $b$ from the line of best fit).

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson08/8_4_CoeffDetermination.html#practice)
