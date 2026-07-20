<head>
<title>Lesson 14.3 Cumulative Binomial Probabilities</title>
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

# Lesson 14.3 Cumulative Binomial Probabilities
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.4.2 Formula for the binomial distribution

## Lesson
We now bring together everything from this lesson. In [lesson 13](../Lesson13/index.html), we learned to find $P(x)$, the probability of **exactly** $x$ successes in a binomial experiment. In lesson 14.2, we learned how to turn a table of individual probabilities into a **cumulative** probability by adding the right terms. Putting these together lets us answer "at least," "at most," "more than," "fewer than," and "between" questions directly for a binomial experiment.

### The Idea

To find a cumulative binomial probability, calculate $P(x)$ with the binomial formula for every value of $x$ that belongs to the range you need, and add them together — exactly as in lesson 14.2, just using $P(x) = \binom{n}{x}p^xq^{n-x}$ for each individual term.

$$P(x) = \binom{n}{x}p^xq^{n-x}$$

### Worked Example

Suppose 30% of customers who enter a store make a purchase ($p=0.30$), and $n=8$ independent customers enter the store. Find the probability that **at most 2** customers make a purchase.

$$P(x\leq 2) = P(0)+P(1)+P(2)$$

$$P(0) = \binom{8}{0}(0.3)^0(0.7)^8 \approx 0.0576$$
$$P(1) = \binom{8}{1}(0.3)^1(0.7)^7 \approx 0.1977$$
$$P(2) = \binom{8}{2}(0.3)^2(0.7)^6 \approx 0.2965$$

$$P(x\leq 2) \approx 0.0576+0.1977+0.2965 = 0.5518$$

There is about a **55.18%** chance that at most 2 of the 8 customers make a purchase.

Now find the probability that **at least 3** customers make a purchase, using the Complement Shortcut from lesson 14.2:

$$P(x\geq 3) = 1-P(x\leq 2) = 1-0.5518 = 0.4482$$

Adding up individual binomial probabilities by hand gets tedious fast, especially for large $n$ — this is exactly the kind of calculation where technology earns its keep.

<iframe width="560" height="315" src="https://www.youtube.com/embed/BME2P9NqioU?si=NkE1QqDpQhBGwR8x" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. A fair coin is flipped 10 times. Find the probability of getting **at most 4** heads.
  - [After solving on your own, see solution here](./Solutions/14_3_Solution1.html)
2. Historically, 15% of packages shipped by a company arrive late. For a random sample of 20 independent packages, find the probability that **at least 5** arrive late.
  - [After solving on your own, see solution here](./Solutions/14_3_Solution2.html)
3. A basketball player makes 75% of her free throws. If she shoots 12 free throws, find the probability that she makes **between 8 and 10** (inclusive).
  - [After solving on your own, see solution here](./Solutions/14_3_Solution3.html)
4. A survey shows that 40% of adults in a town support a proposed tax increase. If 15 adults are randomly and independently selected, find the probability that **more than 8** support the increase.
  - [After solving on your own, see solution here](./Solutions/14_3_Solution4.html)

## Technology

### TI-83/84
1. Press **2ND**, then **VARS** to open the **DISTR** (distributions) menu.
2. Scroll down to **binomcdf(** (cumulative distribution function — this gives the probability of $x$ **or fewer** successes) and press **ENTER**.
3. Enter the values in order: `binomcdf(n, p, x)`, where $n$ is the number of trials, $p$ is the probability of success, and $x$ is the upper bound of the range.
  - This directly gives you $P(x \leq x_0)$, or "at most $x_0$."
  - For "at least $x_0$," use the Complement Shortcut: `1 - binomcdf(n, p, x0 - 1)`.
  - For "between $a$ and $b$" (inclusive), subtract two cumulative probabilities: `binomcdf(n, p, b) - binomcdf(n, p, a - 1)`.
4. Press **ENTER** to see the probability.

<iframe width="560" height="315" src="https://www.youtube.com/embed/g2X1XyF9Sso?si=6bR-3Z1PPh2Pua-K" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Excel
1. Click on an empty cell where you want the result to appear.
2. Type the following formula, then press Enter:
  - `=BINOM.DIST(x, n, p, TRUE)`
3. The **TRUE** tells Excel you want the **cumulative** probability $P(x \leq x_0)$ — "at most $x_0$" successes — rather than the probability of exactly $x_0$.
4. For example, to find $P(x\leq 2)$ for the store example above (8 trials, $p=0.30$): `=BINOM.DIST(2, 8, 0.3, TRUE)`
5. For "at least $x_0$," subtract from 1: `=1-BINOM.DIST(x0-1, n, p, TRUE)`
6. For "between $a$ and $b$" (inclusive), subtract two cumulative values: `=BINOM.DIST(b, n, p, TRUE)-BINOM.DIST(a-1, n, p, TRUE)`

### Desmos
Desmos doesn't have a built-in cumulative binomial function, but we can build one out of a sum, using the same combinations function from lesson 13.2.
1. In a blank expression line, type a sum using Desmos's summation notation:
  - `sum(nCr(n,k)*p^k*(1-p)^(n-k), k, a, b)`
  - Here, $a$ is the lower bound and $b$ is the upper bound of the range of successes you want (both inclusive).
2. For example, to find $P(x\leq 2)$ for the store example above: `sum(nCr(8,k)*0.3^k*0.7^(8-k), k, 0, 2)`
3. Press **Enter**, and Desmos will evaluate the sum for you.
4. For "at least $x_0$" out of $n$ trials, set the lower bound to $x_0$ and the upper bound to $n$.
