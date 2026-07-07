<head>
<title>4.6 Scatterplots</title>
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
canonical: https://drolsonmi.github.io/math1040/Lesson04/4_6_Scatterplots.html
meta-description: Lecture Pages for MATH 1040 Online course
meta-generator: Jekyll v3.10.0
meta-og:description: Lecture Pages for MATH 1040 Online course
meta-og:locale: en_US
meta-og:site_name: MATH 1040 - Introduction to Statistics
meta-og:title: MATH 1040 - Introduction to Statistics
meta-og:type: website
meta-og:url: https://drolsonmi.github.io/math1040/Lesson04/4_6_Scatterplots.html
meta-twitter:card: summary
meta-twitter:title: MATH 1040 - Introduction to Statistics
meta-viewport: width=device-width, initial-scale=1
---

# Lesson 4.6 Scatterplots

## Reading

Reading sections are from the [Introductory Statistics Textbook](https://drolsonmi.github.io/math1040/Resources/OpenIntroTextbook.pdf)

- 1.3.3 Explanatory and Response Variables (page 19)
- 2.1.1 Scatterplots for paired data (pages 46-48)

## Lesson

*A **scatterplot** is used to look at the relationship between two quantitative variables measured on the same set of individuals.* This is different from every other graph we've studied so far in this lesson — dotplots and stemplots only look at one variable at a time. In a scatterplot, we are going to graph two quantitative variables together. One variable will be on the x-axis and the other on the y-axis.

Recall our definition of explanatory and response variables:

- **Explanatory Variable** (also known as **independent variable**): the variable that influences the other variable
- **Response Variable** (also known as **dependent variable**): the variable that is influenced by the explanatory variable

When you compare two quantitative variables, the first thing you need to do is determine which of the two variables is the explanatory variable and which is the response variable. Once you know these, label the x-axis as the explanatory variable and the y-axis as your response variable.

Once your labels are created,

- Take one datapoint and identify its value for the explanatory variable, then find that point on the x-axis
- From the same datapoint, identify its value for the response variable, then find that point on the y-axis
- Imagine a vertical line from your x-value and a horizontal line from your y-value. Where they meet is the location of your datapoint

Do this for all datapoints, and you have a scatterplot!

### Reading a Scatterplot

Once a scatterplot is made, we describe it the same way we describe any distribution: with its **shape**, and any unusual features. For scatterplots specifically, we focus on three things:

1. **Direction (Association)**
  - **Positive association**: as the explanatory variable increases, the response variable tends to increase as well (the cloud of points trends upward, left to right)
  - **Negative association**: as the explanatory variable increases, the response variable tends to decrease (the cloud of points trends downward, left to right)
  - **No association**: there is no visible pattern between the two variables
2. **Form**
  - Do the points roughly follow a straight line (**linear**)?
  - Do they curve (**nonlinear** / **curvilinear**)?
  - Or is there no clear form at all?
3. **Strength**
  - Are the points tightly clustered around a clear pattern (**strong** relationship), or are they scattered loosely with just a general trend (**weak** relationship)?

We should also always look for **outliers** — individual points that fall far away from the overall pattern of the rest of the data.

For example, if we plotted a car's **weight** (explanatory variable) against its **gas mileage** (response variable) using our cars dataset from [4.1 Graphing Basics](https://drolsonmi.github.io/math1040/Lesson04/4_1_GraphingBasics.html), we would expect to see a **negative**, fairly **strong**, roughly **linear** association: heavier cars tend to get fewer miles per gallon. On the other hand, if we plotted a car's **weight** against the **number of doors** it has, we would likely see almost no association at all, since a car's weight doesn't really determine how many doors it has.

### A Word of Caution: Correlation vs. Causation

Just because two variables show a strong association in a scatterplot does *not* mean that one variable **causes** the other to change. There could be another variable (a **lurking variable**) responsible for both, or the relationship could simply be a coincidence. We will discuss this idea in much more detail later in the course, but keep it in mind any time you interpret a scatterplot: *association is not the same thing as causation.*

## Practice

1. A researcher records the number of hours 10 students studied for an exam and their exam score:

| Hours Studied |   1   |   2   |   2   |   3   |   3   |   4   |   5   |   5   |   6   |   7   |
| :------------ | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Exam Score    |  55   |  62   |  68   |  70   |  75   |  78   |  85   |  88   |  90   |  95   |

  - Identify the explanatory and response variables.
  - Create a scatterplot of this data.
  - Describe the direction, form, and strength of the association.
  - [After solving on your own, see solution here](https://drolsonmi.github.io/math1040/Lesson04/Solutions/4_6_Solution1.html)
2. For each pair of variables below, state whether you would expect a positive association, a negative association, or no association, and explain why.
  - A person's age and their resting heart rate
  - The outdoor temperature and the number of hot cocoas sold at a stand
  - A person's shoe size and their favorite color
  - [After solving on your own, see solution here](https://drolsonmi.github.io/math1040/Lesson04/Solutions/4_6_Solution2.html)


## Technology

### Microsoft Excel

<iframe width="560" height="315" src="https://www.youtube.com/embed/nTLAuiRxBPQ?si=cgJPCQsXqCGZEc7j" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>