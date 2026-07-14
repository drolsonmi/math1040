<head>
<title>Solution for practice 11.4.1</title>
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

## 11.4 Combinations - Solution for Practice 1
You're visiting a city with 7 major tourist attractions, and you only have time to visit 3 of them in one day. You want to plan the order in which you'll visit them to make the most of your experience. You plan to spend __equal__ time at each site, so the order doesn't matter. How many options do you have for choosing 3 attractions?

### Answer to Practice Question 11.4.1
If there are 7 attractions and we choose 3 of them. From permutations, there are $${}_7C_3 = 210$$ different arrangements.

Since the order doesn't matter, we divide 210 by the number of rearrangements, 3! = 6.

So, __there are 210/6 = 35 different combinations__.

Looking at the full calculation:

$$
\begin{align*}
    {}_7C_3 &= \frac{7!}{3!(7-3)!} \\
            &= \frac{7!}{3!4!} \\
            &= \frac{~~~7\times 6\times 5\times 4\times 3\times 2\times 1}{(3\times 2\times 1)\times(4\times 3\times 2\times 1)} \\
            &= \frac{7\times 6\times 5}{3\times 2\times 1} \\
            &= \frac{210}{6}\\
            &= \mathbf{35}
\end{align*}
$$
