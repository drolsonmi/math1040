<head>
<title>Lesson 13.3 Binomial Distributions</title>
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

# Lesson 13.3 Binomial Distributions
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 4.3 Binomial Distribution (pages 164-165)

## Lesson
In [lesson 12](../Lesson12/12_1_ProbabilityDistributions.html), we learned that a probability distribution is a table listing every possible value of $r$ along with its probability. Now that we can calculate $P(X=r)$ for a binomial experiment, we can build the entire __binomial probability distribution__ by repeating the formula for every possible value of $r$, from $r=0$ up to $r=n$.

$$P(X=r) = {}_nC_r p^r q^{n-r} \qquad \text{for } r = 0, 1, 2, \dots, n$$

### Worked Example

Suppose a basketball player makes 70% of her free throws ($p = 0.70$), and she shoots $n=4$ free throws. Let $r$ be the number of free throws she makes. Since $r$ can be $0, 1, 2, 3,$ or $4$, we calculate $P(X=r)$ for each value:

$$P(0) = \binom{4}{0}(0.7)^0(0.3)^4 = 1(1)(0.0081) = 0.0081$$
$$P(1) = \binom{4}{1}(0.7)^1(0.3)^3 = 4(0.7)(0.027) = 0.0756$$
$$P(2) = \binom{4}{2}(0.7)^2(0.3)^2 = 6(0.49)(0.09) = 0.2646$$
$$P(3) = \binom{4}{3}(0.7)^3(0.3)^1 = 4(0.343)(0.3) = 0.4116$$
$$P(4) = \binom{4}{4}(0.7)^4(0.3)^0 = 1(0.2401)(1) = 0.2401$$

This gives us the complete binomial distribution:

| $r$      | 0      | 1      | 2      | 3      | 4      |
| :------: | :----: | :----: | :----: | :----: | :----: |
| $P(X=r)$ | 0.0081 | 0.0756 | 0.2646 | 0.4116 | 0.2401 |

### Checking the Distribution

Just like any probability distribution from lesson 12, a binomial distribution must satisfy two rules:
- Every probability is between 0 and 1.
- The probabilities all add up to 1.

$$0.0081 + 0.0756 + 0.2646 + 0.4116 + 0.2401 = 1.0000\checkmark$$

Once we have the full distribution, we can also treat it like any other discrete probability distribution — for example, finding its expected value $\mu = \sum rP(X=r)$, just as we did in lesson 12. In fact, the binomial distribution has a shortcut formula for the mean and standard deviation that will always match what you'd get the long way:

$$\mu = np \qquad \sigma = \sqrt{npq}\tag{Binomial Mean and Standard Deviation}$$

For the free-throw example: $\mu = 4(0.7) = 2.8$ makes and $\sigma = \sqrt{4(0.7)(0.3)} \approx 0.917$.

<iframe width="560" height="315" src="https://www.youtube.com/embed/gCiu-o1e4rI?si=T3fCkYtIPh0DwlBv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. A fair coin is flipped 3 times. Build the complete binomial probability distribution for $x$ = number of heads, and verify that the probabilities sum to 1.
  - [After solving on your own, see solution here](./Solutions/13_3_Solution1.html)
2. In a certain city, 20% of drivers run a red light at a particular intersection. For a random sample of 5 independent drivers passing through the intersection, build the complete binomial distribution for $x$ = number who run the red light. Then find the mean and standard deviation using the shortcut formulas.
  - [After solving on your own, see solution here](./Solutions/13_3_Solution2.html)
3. A pharmaceutical trial shows that a new medication is effective for 60% of patients. For a group of 4 independent patients, build the complete binomial distribution for $r$ = number for whom the medication is effective. Use the distribution to find $P(X \geq 3)$.
  - [After solving on your own, see solution here](./Solutions/13_3_Solution3.html)
