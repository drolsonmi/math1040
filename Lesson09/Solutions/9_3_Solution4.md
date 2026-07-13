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

## 9.3 Complements - Solution for Practice 4

1. A fair coin is flipped twice. Find the probability of getting **at least one heads**, by first finding the probability of the complement (getting zero heads).

### Solution

**Step 1: Write out the sample space.**

Flipping a coin twice gives us 4 equally likely outcomes:

$$\{HH, HT, TH, TT\}$$

**Step 2: Identify the complement of "at least one heads."**

The complement of "at least one heads" is "**zero** heads" — meaning both flips landed tails:

$$A' = \{TT\}$$

This is the whole reason complements are so useful here: "at least one heads" actually includes three different outcomes ($HH$, $HT$, $TH$), but its complement, "zero heads," is just a single simple outcome to identify.

**Step 3: Find $P(A')$.**

$$P(\text{zero heads}) = \frac{1}{4} = 0.25$$

**Step 4: Use the complement rule to find $P(A)$.**

$$P(\text{at least one heads}) = 1 - P(\text{zero heads}) = 1 - 0.25 = 0.75 = 75\%$$

The probability of getting **at least one heads** in two flips is **0.75, or 75%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson09/9_3_Complements.html#practice)
