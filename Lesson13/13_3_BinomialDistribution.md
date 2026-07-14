<head>
<title>Lesson 13.3 Binomial Probability Distribution</title>
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

# Lesson 13.3 Binomial Probability Distribution
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 4.3 Binomial distribution (pages 149-158)

## Lesson
In lesson 13.2, we used the binomial probability formula to find the probability of getting *exactly* one specific number of successes. If we repeat that formula for **every** possible value of $k$, from $0$ up to $n$, we get the full __binomial probability distribution__ — the same kind of probability distribution we built in lesson 12, just with the binomial formula generating each probability.

$$P(X=k) = \binom{n}{k}p^k(1-p)^{n-k} \quad \text{for } k = 0, 1, 2, \dots, n$$

### Building a Distribution Table

Suppose 20% of seeds from a certain packet fail to germinate. If we plant $n=4$ seeds, let $X$ = the number of seeds that fail to germinate. Here, $p = 0.20$. We calculate $P(X=k)$ for every value of $k$ from 0 to 4:

| $x$ | $P(x)$ |
| --- | --- |
| 0 | $\binom{4}{0}(0.2)^0(0.8)^4 = 0.4096$ |
| 1 | $\binom{4}{1}(0.2)^1(0.8)^3 = 0.4096$ |
| 2 | $\binom{4}{2}(0.2)^2(0.8)^2 = 0.1536$ |
| 3 | $\binom{4}{3}(0.2)^3(0.8)^1 = 0.0256$ |
| 4 | $\binom{4}{4}(0.2)^4(0.8)^0 = 0.0016$ |

Just like every probability distribution from lesson 12, notice that all of the probabilities add up to 1:

$$0.4096+0.4096+0.1536+0.0256+0.0016 = 1.0000$$

Also notice the **shape** of this distribution: since $p=0.2$ is far from 0.5, the distribution is skewed, with most of the probability piled up at the low values of $x$ and a long tail toward higher values. When $p$ is close to 0.5, a binomial distribution looks much more symmetric; the farther $p$ is from 0.5 (in either direction), the more skewed the distribution becomes.

### Finding the Probability of a Range of Values

This is where lesson 13.1 comes back into play. Once we have the full distribution — or even just the individual probabilities we need — we can find the probability of a *range* of outcomes by adding up the individual probabilities, because getting exactly one value of $X$ and exactly another value of $X$ are mutually exclusive events.

$$P(a \le X \le b) = P(X=a) + P(X=a+1) + \dots + P(X=b)$$

**Example:** Suppose 15% of people in a certain population are left-handed. In a random sample of 20 people, what is the probability that **3, 4, or 5** of them are left-handed?

Here, $n=20$ and $p=0.15$. We need $P(X=3) + P(X=4) + P(X=5)$:

$$P(X=3) = \binom{20}{3}(0.15)^3(0.85)^{17} \approx 0.2428$$

$$P(X=4) = \binom{20}{4}(0.15)^4(0.85)^{16} \approx 0.1821$$

$$P(X=5) = \binom{20}{5}(0.15)^5(0.85)^{15} \approx 0.1028$$

$$P(3 \le X \le 5) = P(3)+P(4)+P(5) \approx 0.2428+0.1821+0.1028 = 0.5277$$

There is about a **52.8% chance** that 3, 4, or 5 out of the 20 people are left-handed.

Adding up individual probabilities by hand works, but it's slow — especially for a wide range of values. In the Technology section below, you'll see a much faster way to do this using each tool's **cumulative** binomial function, which adds up a whole run of probabilities for you in a single step.

<!-- Insert lesson video here -->

## Practice
1. A basketball player makes 70% of her free throws. She attempts 5 free throws. Build the full binomial probability distribution table for $X$ = the number of free throws made (list $P(x)$ for $x=0,1,2,3,4,5$), and confirm that the probabilities add up to 1.
  - [After solving on your own, see solution here](./Solutions/13_3_Solution1.html)
2. A manufacturer finds that 10% of the widgets it produces are defective. In a random sample of 6 widgets, what is the probability that **at most 2** are defective? (Hint: "at most 2" means $X=0$, $X=1$, or $X=2$.)
  - [After solving on your own, see solution here](./Solutions/13_3_Solution2.html)
3. A call center finds that 25% of incoming calls result in a sale. Out of 15 randomly selected calls, what is the probability that **6, 7, or 8** of them result in a sale?
  - [After solving on your own, see solution here](./Solutions/13_3_Solution3.html)

## Technology

### TI-83/84
To build a full distribution table at once, you can generate a list of $x$-values and let the calculator compute $P(x)$ for the whole list simultaneously.

1. Press **STAT**, then **1: Edit** to open the list editor.
2. In **L1**, enter the values of $x$ (for example, $0, 1, 2, 3, 4$).
3. Highlight the **L2** header, then press **2ND**, **VARS** to open the **DISTR** menu, and select **binompdf(**.
4. Enter `binompdf(n, p, L1)` and press **ENTER**. The calculator fills L2 with $P(x)$ for every value of $x$ in L1 all at once.

To find the probability of a **range** of values (like $P(3 \le X \le 5)$), use the cumulative binomial function, **binomcdf**, which gives $P(X \le k)$:

1. Press **2ND**, **VARS**, and select **binomcdf(**.
2. Enter `binomcdf(n, p, k)` to find $P(X \le k)$.
3. Since $P(3 \le X \le 5) = P(X \le 5) - P(X \le 2)$, calculate `binomcdf(n, p, 5) - binomcdf(n, p, 2)`.
  - Subtracting $P(X \le 2)$ removes everything up through $X=2$, leaving exactly $X=3, 4, 5$.

### Excel
1. To find an individual probability, use `=BINOM.DIST(k, n, p, FALSE)` as shown in lesson 13.2.
2. To build a full distribution table, list your $x$-values down a column (e.g., A1:A6 for $x=0$ through $5$), then in the adjacent column enter `=BINOM.DIST(A1, n, p, FALSE)` and fill it down for each row.
3. To find a cumulative probability $P(X \le k)$, change the last argument to **TRUE**: `=BINOM.DIST(k, n, p, TRUE)`.
4. To find the probability of a range, such as $P(3 \le X \le 5)$, subtract: `=BINOM.DIST(5, n, p, TRUE) - BINOM.DIST(2, n, p, TRUE)`.

### Desmos
1. To build a distribution table, create a list of $x$-values, for example: `x_1 = [0,1,2,3,4]`
2. On the next line, define the probability using the combination formula from lesson 13.2, applied to the whole list at once: `P = nCr(n,x_1)*p^{x_1}*(1-p)^{n-x_1}`
3. Desmos will return a matching list of probabilities, one for each value in `x_1`. You can also plot these as points to visualize the shape of the distribution.
4. For the probability of a range of values, sum the relevant terms directly using Desmos's summation notation: $\sum_{k=3}^{5} nCr(n,k)p^k(1-p)^{n-k}$
