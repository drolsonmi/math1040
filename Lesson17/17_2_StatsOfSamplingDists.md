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
</head>

# 17.2 Statistics of Sampling Distributions

## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 4.2.1 The mean and standard deviation of $\bar{x}$ (pages 155-159)

## Lesson
In lesson 17.1, we saw that if we take a large enough samples to from a sampling distribution, we form a normal distribution.

Now, we need to talk about the exact shape of the normal distribution. Let's consider a new dataset. Am individual's intelligence is measured in America using the IQ test. The distribution has a population mean of 100 ($\mu = 100$) and a standard deviation of 15 ($\sigma = 15$).

Your company collects 10,000 sample averages of people's IQ scores. In the following figures, I show the sampling distributions indicated with the blue histogram and the normal distribution of the samples (red curve). I also show the normal distribution for the population (green curve). The figures show the distributions for sample sizes of 10, 25, 50, and 100.

<img src="./images/Fig17_2a_sampling_distributions.png" width=500 alt="Sampling Distributions compared to normal distributions of the population">

Notice how the mean for the population and the samples are the same. So, 
$$\mu_{\bar{x}} = \mu$$

However, the normal distributions become narrower (they have smaller standard deviations). Let's compare the standard deviations of the two normal distributions. 

When the sample size is n = 10, the standard deviation is $\sigma_{\bar{x}} = 4.748$. If we take the ratio of the standard deviations, 
$$\frac{\sigma}{\sigma_{\bar{x}}} = \frac{15}{4.748} = 3.159$$

At first this doesn't look very helpful. However, when we see that $\sqrt{10}=3.162$, then we have a possible connection! Let's see if this works for our other sample sizes.

| Sample Size ($n$) | $\sigma_{\bar{x}}$ | $\frac{\sigma}{\sigma_{\bar{x}}}$ | $\sqrt{n}$ |
| :---: | :---:|:---:|:---:|
| 10  | 4.748 |  3.159 | 3.162 |
| 25  | 3.012 |  4.980 | 5     |
| 50  | 2.117 |  7.085 | 7.071 |
| 100 | 1.494 | 10.040 | 10    |

The last two columns are the ones we want to look at. The second-to-last column is the ratio of standard deviations, and the last column is $\sqrt{n}$. And they are very close! If the number of samples increases, then the two values will get closer and closer.

So, it holds! We now have a relationship between the population and sampling standard deviations. 
$$\sqrt{n} = \frac{\sigma}{\sigma_{\bar{x}}} \qquad \sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$$

<iframe width="560" height="315" src="https://www.youtube.com/embed/9BsdYjceZjo?si=MUtl0zx60ZTCXzz3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
For each problem, find the mean and standard deviation of the sampling distribution ($\mu_{\bar{x}}$ and $\sigma_{\bar{x}}$).
 
1. A population has a mean of $\mu = 50$ and a standard deviation of $\sigma = 8$. A random sample of size $n = 16$ is taken. Find $\mu_{\bar{x}}$ and $\sigma_{\bar{x}}$.
  - [After solving on your own, see solution here](./Solutions/17_2_Solution1.html)
2. Human body temperature has a population mean of $\mu = 98.6\degree F$ and a standard deviation of $\sigma = 0.7\degree F$. A nurse records the average temperature of a random sample of 49 patients. Find $\mu_{\bar{x}}$ and $\sigma_{\bar{x}}$, and explain in a sentence what $\sigma_{\bar{x}}$ tells you in this context.
  - [After solving on your own, see solution here](./Solutions/17_2_Solution2.html)
3. A machine fills water bottles, and the amount it dispenses has some unknown population standard deviation $\sigma$. A quality control team takes repeated samples of size $n = 36$ bottles, and finds that the resulting sampling distribution has a standard deviation of $\sigma_{\bar{x}} = 3$ mL. What is the population standard deviation $\sigma$?
  - [After solving on your own, see solution here](./Solutions/17_2_Solution3.html)
4. SAT scores for a particular year have a population mean of $\mu = 1050$ and a standard deviation of $\sigma = 200$.
    - Find $\sigma_{\bar{x}}$ for random samples of size $n = 25$.
    - Find $\sigma_{\bar{x}}$ for random samples of size $n = 100$.
    - Compare your two answers. What does this tell you about the relationship between sample size and the spread of a sampling distribution?
  - [After solving on your own, see solution here](./Solutions/17_2_Solution4.html)


## Technology
The calculations in this lesson are straightforward arithmetic: $\mu_{\bar{x}}$ is just the population mean $\mu$, and $\sigma_{\bar{x}}$ is the population standard deviation $\sigma$ divided by the square root of the sample size $n$. Here's how to calculate $\sigma_{\bar{x}} = \dfrac{\sigma}{\sqrt{n}}$ with technology.
 
### TI-83/84
1. From the home screen, type the population standard deviation, then press the division key **÷**.
2. Press **2nd**, then $x^2$ to bring up the square root symbol **√(**.
3. Type the sample size $n$, then close the parenthesis.
  - For example, to calculate $\sigma_{\bar{x}} = \frac{15}{\sqrt{10}}$, type: `15/√(10)`
4. Press **ENTER** to calculate.
### Excel
1. Enter the population standard deviation $\sigma$ into one cell (for example, A1) and the sample size $n$ into another cell (for example, A2).
2. Click on an empty cell where you want $\sigma_{\bar{x}}$ to appear.
3. Type the formula: `=A1/SQRT(A2)`
4. Press Enter. Adjust the cell references to match wherever your values are located.
### Desmos
1. Open a new expression line.
2. Type your population standard deviation, followed by a forward slash `/`, then type `sqrt` (Desmos will automatically create a square root symbol) and enter the sample size inside it.
  - For example, to calculate $\sigma_{\bar{x}} = \frac{15}{\sqrt{10}}$, type: `15/sqrt(10)`
3. Press **Enter**. Desmos will display the decimal result immediately to the right of the expression.
 