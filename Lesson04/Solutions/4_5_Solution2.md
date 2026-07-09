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
<title>Solution for practice 4.5.2</title>
</head>

## 4.5 Stem-and-leaf plots - Solution for Practice 2
 
2. Using the stemplot you created in Problem 1, answer the following:
  - How many people were on hold for fewer than 20 minutes?
  - What is the longest hold time in the data?
  - Describe the shape of the distribution in a sentence.

### Solution
 
Recall the stemplot from Problem 1:
 
```
Minutes on Hold (n = 15)
Stem | Leaf
  0  | 8 9
  1  | 1 2 4 5 8 9
  2  | 1 2 5 7 9
  3  | 1 3
 
Key: 1|2 = 12
```
 
- **Fewer than 20 minutes**: this includes every leaf on the "0" and "1" stems: 8, 9, 11, 12, 14, 15, 18, 19. That's **8 people**.
- **Longest hold time**: the largest leaf on the largest stem is on the "3" row: 31 and 33. The longest hold time is **33 minutes**.
- **Shape**: the distribution is fairly symmetric and mound-shaped, centered in the high-teens to low-twenties, with no obvious outliers.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson04/4_5_Stemplots.html#practice)