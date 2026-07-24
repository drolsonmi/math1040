<head>
<script>
MathJax = {
  tex: {
    inlineMath: [['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']]
  }
};
</script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 17: The Central Limit Theorem
e have arrived at the __Central Limit Theorem__. I cannot define it here yet. This theorem will take some time to build up to. For now, just know that it is absolutely critical to statistics. It is what links our information that we gather from samples back to the populations they came from. It is the reason why our polls from political compaigns help us understand who is going to win elections long before the counting is completed.
 
Up to this point in the course, we have learned about samples.
* Segment 1: Variables, Sampling Methods, Study Design, Graphing
* Segment 2: Analysis of Quantitative Variables
* Segment 3: Analysis of Categorical Variables using Probabilities
In lesson 15, we learned about Normal Distributions. This will be a critical tool moving forward. In lesson 17, we are going to use normal distributions to learn about the crux of statistics: the __Central Limit Theorem__.
 
Imagine you are doing a study on the average height of American females, which is 5 feet 3.5 inches (this would be a population mean).
 
If you were to randomly select one woman, the chance of her height being near 5 feet 3.5 inches (the population mean) is pretty high. The chance of her height being over 6 feet is low. Not really low, but definitely less probable than a height near the population mean.
 
Now, if you instead randomly select 4 women, the chances of their mean height (the sample mean) being 6 feet tall or higher is quite low.
 
Randomly selecting 10 women whose sample mean height is over 6 feet tall is so extremely small it is nearly impossible.
 
Larger samples lead to lower probabilities that the sample mean is an extreme value, and more likely that the sample mean is near the population mean.
 
This is the principle of the __Central Limit Theorem__. If we can create a sample large enough, then our sample can more accurately approximate the population. In Lesson 17, we will study more about how the Central Limit Theorem works, then begin implementing it in lessons 18 and 19.


<iframe width="560" height="315" src="https://www.youtube.com/embed/j6B8HzVTytc?si=6TWRRy3RzIIzhCDd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Outcomes
 
By the end of this lesson, you should be able to accomplish the following:
 
- Explain what a sampling distribution is and how it is built from repeated samples of a population
- Describe how the shape of a sampling distribution changes as the sample size increases
- Calculate the mean and standard deviation of a sampling distribution ($\mu_{\bar{x}}$ and $\sigma_{\bar{x}}$) from the population parameters
- State the Central Limit Theorem and check whether its conditions are satisfied for a given scenario
- Use the Central Limit Theorem to calculate probabilities for sample means, and compare them to probabilities for single values


## Topics in this lecture
- [17.1 Sampling Distributions](./17_1_SamplingDistributions.md)
- [17.2 Statistics of Sampling Distributions](./17_2_StatsOfSamplingDists.md)
- [17.3 The Central Limit Theorem](./17_3_CentralLimitTheorem.md)
- [17.4 Example of using the Central Limit Theorem](./17_4_Example.md)