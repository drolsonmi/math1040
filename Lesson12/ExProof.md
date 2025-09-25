<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Proof that the expected value is the same as the mean.
In our lesson material, I claimed that the equation for the expected value is the same as the equation for the mean. On this page, I'll show you that they are, in fact, the same.

Here is the equation for the mean:

$$\bar{x} = \frac{x_1 + x_2 + x_3 + \dots}{n}$$

> For an example, we take this dataset: \{15, 16, 16, 17, 18, 18, 18, 19, 20, 21\}.
>
> $$\bar{x} = \frac{15+16+16+17+18+18+18+19+20+21}{10} = \frac{178}{10} = 17.8$$

We can separate this fraction by dividing each term in the numerator individually by the denominator. This is the same as multiplying it by 1/n.

$$\bar{x} = x_1\frac{1}{n} + x_2\frac{1}{n} + x_3\frac{1}{n} + \dots$$

What if a certain value is repeated? We'll say that $$x_i$$ is in our dataset $$m_i$$ times.

$$\bar{x} = x_1\frac{m_1}{n} + x_2\frac{m_2}{n} + x_3\frac{m_3}{n} + \dots$$

But that fraction $$\tfrac{m_i}{n}$$ is just the relative frequency of the value $$x_i$$. We use the relative frequency as the probability. So,

$$\bar{x} = x_1\cdot P(x_1) + x_2\cdot P(x_2) + x_3\cdot P(x_3) + \dots = \sum x_i\cdot P(x_i) = E[X]$$

> Create a probability distribution of our sample dataset:
> 
> | Value     |  15   |  16   |  17   |  18   |  19   |  20   |  21   |
> | :-------- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
> | Frequency | 1/10  | 2/10  | 1/10  | 3/10  | 1/10  | 1/10  | 1/10  |
>
> $$E[X] = \mu = 15\left(\frac{1}{10}\right) + 16\left(\frac{2}{10}\right) + 17\left(\frac{1}{10}\right) + 18\left(\frac{3}{10}\right) + 19\left(\frac{1}{10}\right) + 20\left(\frac{1}{10}\right) + 21\left(\frac{1}{10}\right)$$
> $$E[X] = \frac{15}{10} + \frac{32}{10} + \frac{17}{10} + \frac{54}{10} + \frac{19}{10} + \frac{20}{10} + \frac{21}{10}$$
> $$E[X] = \frac{178}{10} = 17.8$$