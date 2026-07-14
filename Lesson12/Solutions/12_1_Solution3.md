<head>
<title>Solution for practice 12.1.3</title>
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

## 12.1 Probability Distributions - Solution for Practice 3
Here are three distributions. One of them is invalid. Determine which is the invalid distribution and what can be done to fix it.

| Distribution 1 |   A   |   B   |   C   |   D   |   E   |   F   |
| :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
| Probability    | 0.24  | 0.28  | 0.24  | 0.19  | -0.11 | 0.16  |

| Distribution 2 |   A   |   B   |   C   |   D   |   E   |   F   |
| :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
| Probability    | 0.04  | 0.09  | 0.13  | 0.16  | 0.26  | 0.32  |

| Distribution 3 |   A   |   B   |   C   |   D   |   E   |   F   |
| :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
| Probability    | 0.13  | 0.17  | 0.24  | 0.21  | 0.16  | 0.09  |


### Answer to Practice Question 9.2.1
Let's start by finding the sums of each distribution.

Here is the sum of Distribution 1:
$$0.24+0.28+0.24+0.19+(-0.11)+0.16=1.00$$

Here is the sum of Distribution 2:
$$0.04+0.09+0.13+0.16+0.26+0.32 = 1.00$$

Here is the sum of Distribution 3:
$$0.13+0.17+0.24+0.21+0.16+0.09 = 1.00$$

The probabilities in all three distributions add up to 1.0. So, they all pass that test.

However, $$P(E) = -0.11$$ in Distribution 1. All probabilities need to be between 0 and 1, so __distribution 1 is invalid__.