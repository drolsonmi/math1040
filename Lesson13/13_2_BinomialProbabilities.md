<head>
<title>Lesson 13.2 Binomial Probabilities</title>
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

# Lesson 13.2 Binomial Probabilities
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 3.3.1 Understanding the formula (pages 111-112)
* 3.3.2 When and how to apply the formula (pages 112-114)
* 3.3.3 Calculator: binomial probabilities (pages 114-115)

## Lesson
Now that we can recognize a binomial experiment, we want to actually calculate the probability of getting __exactly__ $r$ successes out of $n$ trials.

### Where the Formula Comes From

Think about flipping a coin ($p=0.5$) 3 times and wanting exactly 2 heads. One way this could happen is HHT. Using the multiplication rule for independent events, the probability of that *specific order* is $P(HHT) = p \cdot p \cdot q = p^2q$. But HHT isn't the only way to get 2 heads out of 3 flips — HTH and THH also work. There are ${}_3C_2=3$ different orders that give exactly 2 heads, and each order has the same probability $p^2q$. So:

$$P(2 \text{ heads}) = {}_3C_2 p^2 q^1$$

This is the idea behind the __binomial probability formula__: count how many *ways* (orders) we can arrange $x$ successes among $n$ trials, using combinations, and multiply by the probability of any *one* of those specific orders.

### The Binomial Probability Formula

$$P(X = r) = {}_nC_r p^r q^{n-r} = {}_nC_r p^r (1-p)^{n-r}\tag{Binomial Probability}$$

where
- $n$ = number of trials
- $r$ = number of successes we want
- $p$ = probability of success on a single trial
- $q = 1-p$ = probability of failure on a single trial
- ${}_nC_r = \dfrac{n!}{r!(n-r)!}$ = the number of ways to arrange $r$ successes among $n$ trials

### Worked Example

Suppose 30% of customers who enter a store make a purchase ($p=0.30$), and 8 independent customers enter the store ($n=8$). What is the probability that **exactly 3** of them make a purchase?

$$P(3) = \binom{8}{3}(0.30)^3(0.70)^5$$

$$\binom{8}{3} = 56, \qquad (0.30)^3 = 0.027, \qquad (0.70)^5 \approx 0.16807$$

$$P(3) = 56(0.027)(0.16807) \approx 0.2541$$

There is about a **25.4%** chance that exactly 3 of the 8 customers make a purchase.

<iframe width="560" height="315" src="https://www.youtube.com/embed/8idr1WZ1A7Q?si=lHqQ0_Fh1jvxU9tJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. A fair coin is flipped 6 times. Find the probability of getting exactly 4 heads.
  - [After solving on your own, see solution here](./Solutions/13_2_Solution1.html)
2. A multiple-choice quiz has 10 questions, each with 4 answer choices. A student guesses randomly on every question. Find the probability that the student gets exactly 3 questions correct.
  - [After solving on your own, see solution here](./Solutions/13_2_Solution2.html)
3. A manufacturer knows that 5% of the light bulbs it produces are defective. In a random sample of 12 bulbs, find the probability that exactly 2 are defective.
  - [After solving on your own, see solution here](./Solutions/13_2_Solution3.html)
4. According to a survey, 65% of adults in a city support a new recycling program. If 9 adults are randomly and independently selected, find the probability that exactly 6 of them support the program.
  - [After solving on your own, see solution here](./Solutions/13_2_Solution4.html)

## Technology

### TI-83/84
1. Press **2ND**, then **VARS** to open the **DISTR** (distributions) menu.
2. Scroll down to **binompdf(** (probability density function — this gives the probability of an *exact* number of successes) and press **ENTER**.
3. Enter the values in order: `binompdf(n, p, x)`, where $n$ is the number of trials, $p$ is the probability of success, and $x$ is the exact number of successes you want.
4. Press **ENTER** to see the probability.

<iframe width="560" height="315" src="https://www.youtube.com/embed/N8Kfw2E9ONc?si=B5uYQoxg1uUEr2Y6" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Excel
1. Click on an empty cell where you want the result to appear.
2. Type the following formula, then press Enter:
  - `=BINOM.DIST(x, n, p, FALSE)`
3. Here, $x$ is the exact number of successes, $n$ is the number of trials, and $p$ is the probability of success. The **FALSE** tells Excel you want the probability of *exactly* $x$ successes (not cumulative).
4. For example, to find the probability of exactly 3 successes out of 8 trials with $p=0.30$: `=BINOM.DIST(3, 8, 0.3, FALSE)`

### Desmos
Desmos doesn't have a dedicated binomial probability button, but it can compute the formula directly since it has a built-in combinations function.
1. In a blank expression line, type: `nCr(n,x) * p^x * (1-p)^(n-x)`, replacing $n$, $p$, and $x$ with your values.
  - For example, for the store example above: `nCr(8,3)*0.3^3*0.7^5`
2. Press **Enter**, and Desmos will evaluate the expression for you.
