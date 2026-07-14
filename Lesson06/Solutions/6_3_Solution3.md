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
<title>Solution for practice 6.3.3</title>
</head>

## 6.3 Median - Solution for Practice 3

3. Consider the dataset \[5, 6, 6, 7, 8, 50\].
  - Find the mean, median, and mode of this dataset.
  - Which measure of center best represents a "typical" value in this dataset? Explain why.
{:start="3"}

### Solution

**Mean**:

$$\bar{x} = \dfrac{5+6+6+7+8+50}{6} = \dfrac{82}{6} \approx 13.67$$

**Median**: The dataset is already ordered: \[5, 6, 6, 7, 8, 50\]. There are 6 values, so the median is the average of the 3rd and 4th values:

$$\text{Median} = \dfrac{6+7}{2} = 6.5$$

**Mode**: The value 6 appears twice, more than any other value, so the mode is **6**.

**Which is best?** The mean ($\approx 13.67$) is pulled far above where most of the data actually sits, because of the extreme value 50. Five of the six values are between 5 and 8, so a "typical" value should be somewhere in that range. Both the median (6.5) and the mode (6) fall right in that range, while the mean does not. So in this case, the **median** (or the mode) is a better representation of the typical value than the mean, since it is not distorted by the outlier.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson06/6_3_Median.html#practice)
