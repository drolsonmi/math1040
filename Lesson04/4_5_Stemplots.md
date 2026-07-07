<head>
<title>4.5 Stem-and-Leaf plots</title>
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

---
canonical: https://drolsonmi.github.io/math1040/Lesson04/4_5_Stemplots.html
meta-description: Lecture Pages for MATH 1040 Online course
meta-generator: Jekyll v3.10.0
meta-og:description: Lecture Pages for MATH 1040 Online course
meta-og:locale: en_US
meta-og:site_name: MATH 1040 - Introduction to Statistics
meta-og:title: MATH 1040 - Introduction to Statistics
meta-og:type: website
meta-og:url: https://drolsonmi.github.io/math1040/Lesson04/4_5_Stemplots.html
meta-twitter:card: summary
meta-twitter:title: MATH 1040 - Introduction to Statistics
meta-viewport: width=device-width, initial-scale=1
title: MATH 1040 - Introduction to Statistics | Lecture Pages for MATH 1040 Online course
---

# Lesson 4.5 Stem-and-leaf plots (stemplots)

## Reading

Reading sections are from the [Introductory Statistics Textbook](https://drolsonmi.github.io/math1040/Resources/OpenIntroTextbook.pdf)

- 2.1.2 Stem-and-leaf plots and dot plots (pages 48-49)

## Lesson

Like a dotplot, *a **stem-and-leaf plot** (or a stemplot for short) is used to look at the frequency of a single quantitative variable.* The difference is that instead of looking at the count of one value, we are looking at the count of values in a group of 10 (count of values between 0-9, 10-19, 20-29, 30-39, etc.).

A stemplot splits each data value into two parts:

- The **stem**: all digits except the last one (this represents the "tens" grouping, or higher)
- The **leaf**: the last digit of the value

The stems are lined up in a column (smallest at the top, largest at the bottom), and a vertical line is drawn to their right. For each data value, we write its leaf next to its stem. This groups our data into intervals of 10 while still preserving every single original value (something a bargraph or histogram cannot do).

### Steps to Create a Stemplot

1. Look at the range of the data (find the minimum and maximum) and decide what the stems will be. **This is our scale**, so be sure it is consistent — every stem from the smallest to the largest must be listed, even if a stem ends up with no leaves.
2. Draw a vertical line to the right of the stems.
3. **Label** the plot with a title, and include a key showing how to read a stem-leaf pair (for example, "4|7 = 47").
4. Go through the data values in order and write each leaf next to its stem, from smallest leaf to largest.

### Example

Suppose we record the scores of 20 students on a quiz (out of 100 points):

\[62, 71, 74, 68, 90, 85, 77, 73, 81, 95, 66, 72, 88, 79, 84, 91, 76, 63, 89, 70\]

The smallest value is 62 and the largest is 95, so our stems will run from 6 to 9 (representing the 60s, 70s, 80s, and 90s). Here is the completed stemplot:

```
Quiz Scores (n = 20)
Stem | Leaf
  6  | 2 3 6 8
  7  | 0 1 2 3 4 6 7 9
  8  | 1 4 5 8 9
  9  | 0 1 5

Key: 6|2 = 62
```

Reading this plot, we can quickly see:

- Most students scored in the 70s (8 out of 20 students)
- The lowest score was 62, and the highest was 95
- The data is roughly spread across the 60s through 90s without one score being wildly separate from the rest (no obvious outliers)

Notice that a stemplot turned on its side looks very much like a bar graph or histogram — the length of each row of leaves acts like the height of a bar. This is why a stemplot is so useful: it shows the *shape* of the distribution while still keeping every individual data value visible.

### Back-to-Back Stemplots

Sometimes we want to compare two groups using the same stems. We can do this with a **back-to-back stemplot**, where one group's leaves are written to the left of the stem (read right-to-left) and the other group's leaves are written to the right of the stem (read left-to-right):

```
         Section A  | Stem |  Section B
             9 7 2  |  6   |  3 8
       8 6 4 3 1 0  |  7   |  0 2 5 9
             8 5 1  |  8   |  1 4 8 9
                 0  |  9   |  1 5

            Key: 9|0 = 90
```

This lets us compare the shape and spread of two distributions side by side while keeping the same scale for both.

### When *Not* to Use a Stemplot

Stemplots work well for small to medium datasets (roughly under 50 values) with a reasonable number of digits. If a dataset is very large, or the values have many digits (for example, salaries in the hundreds of thousands), a stemplot becomes cluttered and hard to read. In those cases, a histogram (which we'll cover in Lesson 5) is usually a better choice.

## Practice

1. The following data set shows the number of minutes 15 people spent on hold with customer service:   \[12, 25, 8, 31, 19, 22, 14, 27, 9, 33, 18, 21, 15, 29, 11\]   Create a stem-and-leaf plot for this data. Be sure to include a key.
  - [After solving on your own, see solution here](https://drolsonmi.github.io/math1040/Lesson04/Solutions/4_5_Solution1.html)
2. Using the stemplot you created in Problem 1, answer the following:
  - How many people were on hold for fewer than 20 minutes?
  - What is the longest hold time in the data?
  - Describe the shape of the distribution in a sentence.
  - [After solving on your own, see solution here](https://drolsonmi.github.io/math1040/Lesson04/Solutions/4_5_Solution2.html)

## Technology

### Microsoft Excel

<iframe width="560" height="315" src="https://www.youtube.com/embed/4mmNoHQ1F9Q?si=k7wMB1zdEcU1_OYJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>