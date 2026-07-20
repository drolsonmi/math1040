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
<title>Solution for practice 13.3.2</title>
</head>

## 13.3 Binomial Distributions - Solution for Practice 2
2. In a certain city, 20% of drivers run a red light at a particular intersection. For a random sample of 5 independent drivers passing through the intersection, build the complete binomial distribution for $x$ = number who run the red light. Then find the mean and standard deviation using the shortcut formulas.

### Solution

Here $n=5$, $p=0.2$, $q=0.8$, and $x$ can be $0,1,2,3,4,5$.

$$P(0) = \binom{5}{0}(0.2)^0(0.8)^5 = 1(1)(0.32768) = 0.3277$$
$$P(1) = \binom{5}{1}(0.2)^1(0.8)^4 = 5(0.2)(0.4096) = 0.4096$$
$$P(2) = \binom{5}{2}(0.2)^2(0.8)^3 = 10(0.04)(0.512) = 0.2048$$
$$P(3) = \binom{5}{3}(0.2)^3(0.8)^2 = 10(0.008)(0.64) = 0.0512$$
$$P(4) = \binom{5}{4}(0.2)^4(0.8)^1 = 5(0.0016)(0.8) = 0.0064$$
$$P(5) = \binom{5}{5}(0.2)^5(0.8)^0 = 1(0.00032)(1) = 0.0003$$

| $x$ | 0 | 1 | 2 | 3 | 4 | 5 |
| --- | --- | --- | --- | --- | --- | --- |
| $P(x)$ | 0.3277 | 0.4096 | 0.2048 | 0.0512 | 0.0064 | 0.0003 |

**Check:** $0.3277+0.4096+0.2048+0.0512+0.0064+0.0003 = 1.0000\checkmark$

**Mean and standard deviation**, using the shortcut formulas:

$$\mu = np = 5(0.2) = 1$$

$$\sigma = \sqrt{npq} = \sqrt{5(0.2)(0.8)} = \sqrt{0.8} \approx 0.894$$

On average, we expect 1 out of every 5 drivers to run the red light, with a standard deviation of about 0.894 drivers.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_3_BinomialDistribution.html#practice)
