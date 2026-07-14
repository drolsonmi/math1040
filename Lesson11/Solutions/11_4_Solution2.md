<head>
<title>Solution for practice 11.4.2</title>
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

## 11.4 Combinations - Solution for Practice 2
A business has 9 applicants for 2 job openings, both as managers. How many ways can the business select 2 new employees out of the 9 candidates?

### Answer to Practice Question 11.4.2
Since the job positions are exactly the same, the order doesn't matter. So, to find the number of ways 2 new employees can be selected from a group of 9 candidates, we find the number of permutations:
$${}_9P_2 = 72$$

then divide this by the number of arrangements, which is 2! = 2. There are $${}_9C_2 = 72/2 = 36$$ different combinations.

Looking at the full calculation:

$$
\begin{align*}
    {}_9C_2 &= \frac{9!}{2!(9-2)!} \\
            &= \frac{9!}{2!7!} \\
            &= \frac{~~~~9\times 8\times 7\times 6\times 5\times 4\times 3\times 2\times 1}{(2\times 1)\times(7\times 6\times 5\times 4\times 3\times 2\times 1)} \\
            &= \frac{9\times 8}{2\times 1} \\
            &= \frac{72}{2} \\
            &= \mathbf{36}
\end{align*}
$$
