<head>
<title>Solution for practice 12.3.1</title>
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

## 12.3 Expected Value - Solution for Practice 1

1. A game costs $5 to play. There is a 30% chance of winning $20 (a net gain of $15 after paying to play), and a 70% chance of winning nothing (a net loss of $5). Find the expected value of playing this game, and explain what it means.

### Solution

**Step 1: Set up the table of values and probabilities.** We use the *net* result of playing (winnings minus the $5 cost), not just the raw prize amount.

| Category | Win | Lose |
| --- | --- | --- |
| Value ($x$) | $15 | -$5 |
| Probability ($P(x)$) | 0.30 | 0.70 |

**Step 2: Multiply each value by its probability.**

| Category | Win | Lose |
| --- | --- | --- |
| $x \cdot P(x)$ | $15(0.30) = 4.50$ | $-5(0.70) = -3.50$ |

**Step 3: Add up the results.**

$$E[x] = 4.50 + (-3.50) = 1.00$$

**Interpretation**: The expected value is **$1.00**. This means that if you played this game many, many times, you would expect to come out ahead by about $1 per game, on average. This doesn't mean you'll win exactly $1 every time you play (you'll actually win $15 or lose $5 on any given play) — it means that if you averaged your results over a large number of plays, you'd expect that average to settle in around $1 of profit per game.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson12/12_3_ExpectedValue.html#practice)
