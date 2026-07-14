<head>
<title>Solution for practice 11.3.2</title>
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

## 11.3 Permutations - Solution for Practice 2
A business has 9 applicants for 2 job openings, one as a manager and another as just a regular employee. How many ways can the business select 2 new employees out of the 9 candidates?

### Answer to Practice Question 11.3.2
To find the number of ways 2 new employees can be selected from a group of 9 candidates,

$$
\begin{align*}
    {}_9P_2 &= \frac{9!}{(9-2)!} \\
            &= \frac{9!}{7!} \\
            &= \frac{9\times 8\times 7\times 6\times 5\times 4\times 3\times 2\times 1}{~~~~~~~~~~~~~~7\times 6\times 5\times 4\times 3\times 2\times 1} \\
            &= 9\times 8 \\
            &= \mathbf{72}
\end{align*}
$$
