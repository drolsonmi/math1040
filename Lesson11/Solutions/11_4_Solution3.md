<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice Question 11.4.3
An emergency room receives 8 patients after a multi-vehicle accident. Due to limited resources, only 5 trauma bays are immediately available for treatment. Assume the severity of the injuries is about the same for each patient. In how many different ways can the ER staff choose and prioritize 5 patients out of the 8 for immediate treatment?

### Answer to Practice Question 11.4.3
If there are 8 patients and we only treat 5 at a time.

$$ {}_8P_5 = 6720 $$

There are 5! = 120 different ways to arrange the chosen 5, so the total number of combinations is ${}_8C_5 =$ 6720/120 = 56.

Looking at the full calculations:

$$
\begin{align*}
    {}_8C_5 &= \frac{8!}{5!(8-5)!} \\
            &= \frac{8!}{5!3!} \\
            &= \frac{~~~8\times 7\times 6\times 5\times 4\times 3\times 2\times 1}{(5\times 4\times 3\times 2\times 1)\times (3\times 2\times 1)} \\
            &= \frac{8\times 7\times 6\times 5\times 4}{5\times 4\times 3\times 2\times 1} \\
            &= \frac{6720}{120} \\
            &= \mathbf{56}
\end{align*}
$$