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
<title>Solution for practice 4.5.1</title>
</head>

## 4.5 Stem-and-leaf plots - Solution for Practice 1
 
1. The following data set shows the number of minutes 15 people spent on hold with customer service: \[12, 25, 8, 31, 19, 22, 14, 27, 9, 33, 18, 21, 15, 29, 11\] Create a stem-and-leaf plot for this data. Be sure to include a key.

### Solution
 
First, sort the data from smallest to largest:
 
$$8, 9, 11, 12, 14, 15, 18, 19, 21, 22, 25, 27, 29, 31, 33$$
 
The smallest value is 8 and the largest is 33, so our stems will run from 0 to 3 (representing the ones, teens, twenties, and thirties). Splitting each value into a stem (all digits but the last) and a leaf (the last digit) gives us:
 
```
Minutes on Hold (n = 15)
Stem | Leaf
  0  | 8 9
  1  | 1 2 4 5 8 9
  2  | 1 2 5 7 9
  3  | 1 3
 
Key: 1|2 = 12
```
 
Be sure that your stemplot:
 
- includes every stem from smallest to largest, even if some end up with very few leaves
- includes leaves listed in increasing order within each stem
- has the leaves lined up to accurately show the patterns
- includes a key showing how to read a stem-leaf pair

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson04/4_5_Stemplots.html#practice)