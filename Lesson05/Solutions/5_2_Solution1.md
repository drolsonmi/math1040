<head>
<title>Solution for 5.2.1</title>
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

## 5.2 Creating a Histogram - Solution for Practice 1

1. The ages of 12 customers at a coffee shop were recorded:

$$22, ~24, ~25, ~29, ~31, ~33, ~35, ~38, ~40, ~44, ~47, ~50$$

Follow the steps above to find the range, the number of bins, and the bin size, and then create a histogram of this data.

### Solution

**Step 1: Find the range.**

$$Range = Maximum - Minimum = 50 - 22 = 28$$

**Step 2: Determine the number of bins.**

Our sample size is $n = 12$. Doubling from 1:

$$1 \rightarrow 2 \rightarrow 4 \rightarrow 8 \rightarrow 16$$

We need 4 doublings to reach or pass 12 (since $8 < 12$ but $16 \geq 12$), so we will use **4 bins**.

**Step 3: Create the bins.**

$$Bin~Size = \frac{Range}{\text{number of bins}} = \frac{28}{4} = 7$$

Starting at the minimum value of 22 and adding 7 repeatedly:

| Bin # | Bin Range |
| ----- | --------- |
| 1     | 22 - 29   |
| 2     | 29 - 36   |
| 3     | 36 - 43   |
| 4     | 43 - 50   |

**Step 4: Count your data.**

| Bin Range | Values in Bin      | Frequency |
| --------- | -------------------- | --------- |
| 22 - 29   | 22, 24, 25            | 3         |
| 29 - 36   | 29, 31, 33, 35         | 4         |
| 36 - 43   | 38, 40                 | 2         |
| 43 - 50   | 44, 47, 50             | 3         |

Check: $3 + 4 + 2 + 3 = 12$. This matches our sample size. ✓

**Steps 5 & 6: Draw the histogram.**

![Ages of 12 Customers](https://drolsonmi.github.io/math1040/Lesson05/images/Fig5_2_Practice1_Solution.png)

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson05/5_2_CreatingAHistogram.html#practice)
