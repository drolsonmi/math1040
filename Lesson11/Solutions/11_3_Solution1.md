<head>
<title>Solution for practice 11.3.1</title>
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

## 11.3 Permutations - Solution for Practice 1
You're visiting a city with 7 major tourist attractions, and you only have time to visit 3 of them in one day. You want to plan the order in which you'll visit them to make the most of your experience. You plan to spend the most time in the 1st choice and the least in the 3rd. How many options do you have for choosing 3 attractions?

### Answer to Practice Question 11.3.1
If there are 7 attractions and we choose 3 of them, then,

$$
\begin{align*}
    {}_7P_3 &= \frac{7!}{(7-3)!} \\
            &= \frac{7!}{4!} \\
            &= \frac{7\times 6\times 5\times 4\times 3\times 2\times 1}{~~~~~~~~~~~~~~~~~~~~~4\times 3\times 2\times 1} \\
            &= 7\times 6\times 5 \\
            &= \mathbf{210}
\end{align*}
$$
