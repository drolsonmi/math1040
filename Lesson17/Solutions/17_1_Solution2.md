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
<title>Solution for practice 17.1.2</title>
</head>

## 17.1 Sampling Distributions - Solution for Practice 2
2. Two fair coins are flipped at the same time, and the number of heads (0, 1, or 2) is recorded.
    - List all the possible outcomes of flipping 2 coins, and use them to find the probability of getting 0 heads, 1 head, and 2 heads.
    - Is the resulting distribution symmetric, right-skewed, or left-skewed?

### Solution

**Step 1: List the possible outcomes.**

When 2 coins are flipped, there are 4 equally likely outcomes:

$$HH, \quad HT, \quad TH, \quad TT$$

**Step 2: Count the number of heads in each outcome.**

| Outcome | Number of Heads |
| :---: | :---: |
| HH | 2 |
| HT | 1 |
| TH | 1 |
| TT | 0 |

**Step 3: Find the probability of each value.**

$$P(0 \text{ heads}) = \frac{1}{4} = 0.25$$
$$P(1 \text{ head}) = \frac{2}{4} = 0.50$$
$$P(2 \text{ heads}) = \frac{1}{4} = 0.25$$

**Step 4: Describe the shape.**

The probabilities are $0.25, 0.50, 0.25$ for 0, 1, and 2 heads. This distribution is **symmetric** - it is a mirror image of itself around the middle value of 1 head, with equal probability on either side.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson17/17_1_SamplingDistributions.html#practice)
