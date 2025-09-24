<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice Question 11.3.3
An emergency room receives 8 patients after a multi-vehicle accident. Due to limited resources, only 5 trauma bays are immediately available for treatment. The order in which patients are treated matters because of varying injury severity, risk of complications, and the need for specific specialists. In how many different ways can the ER staff choose and prioritize 5 patients out of the 8 for immediate treatment?

### Answer to Practice Question 11.3.3
If there are 8 patients and we only treat 5 at a time,

$$
\begin{align*}
    {}_8P_5 &= \frac{8!}{(8-5)!} \\
            &= \frac{8!}{3!} \\
            &= \frac{8\times 7\times 6\times 5\times 4\times 3\times 2\times 1}{~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~3\times 2\times 1} \\
            &= 8\times 7\times 6\times 5\times 4 \\
            &= \mathbf{6720}
\end{align*}
$$