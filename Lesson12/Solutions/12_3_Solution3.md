<head>
<title>Solution for practice 12.3.3</title>
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

## 12.3 Expected Value - Solution for Practice 3

1. An insurance company sells a policy for $200 per year. There is a 2% chance a policyholder will file a claim for $5,000 in a given year, and a 98% chance no claim is filed. Find the insurance company's expected payout per policy, and find the company's expected profit per policy.

### Solution

**Step 1: Set up the table of values and probabilities** for the company's *payout* (how much the company pays out, not the premium it collects).

| Category | Claim Filed | No Claim |
| --- | --- | --- |
| Value ($x$) | $5,000 | $0 |
| Probability ($P(x)$) | 0.02 | 0.98 |

**Step 2: Multiply each value by its probability.**

| Category | Claim Filed | No Claim |
| --- | --- | --- |
| $x \cdot P(x)$ | $5000(0.02) = 100$ | $0(0.98) = 0$ |

**Step 3: Add up the results to find the expected payout.**

$$E[\text{payout}] = 100 + 0 = 100$$

The insurance company's **expected payout is $100 per policy**.

**Step 4: Find the expected profit.** The company collects a $200 premium per policy, and expects to pay out $100 per policy on average:

$$\text{Expected profit} = \text{Premium} - E[\text{payout}] = 200 - 100 = 100$$

The insurance company's **expected profit is $100 per policy**. This is exactly how insurance companies set their premiums — high enough, on average, to more than cover the payouts they expect to make, even though any *individual* policyholder either pays $200 and receives nothing, or pays $200 and receives a $5,000 payout.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson12/12_3_ExpectedValue.html#practice)
