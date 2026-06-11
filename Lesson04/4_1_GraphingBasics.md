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

# Lesson 4.1 Graphing Basics

## Lesson
Why do we have graphs? Graphs make it so we as researchers can visualize the data. More importantly, graphs allow our readers to more easily understand the data. Our main audience includes those reading our work. Graphs need to be done in a way that our readers can clearly understand and see our point.

My basic rule of thumb for a graph is this: If I can hand the graph to someone and they can read and understand the graph without asking any questions, then the graph is good. To do this, there are two basic elements that every single graph must have:
1. __A Scale__: Every graph needs a numberline. The numberline helps our readers understand not only the values of a datapoint but also how it compares to other datapoints.
    * Start every graph by examining the range of our data (note the minimum and maximum values)
    * Create a numberline that encases that range
2. __Labels__: Graphs are useless if we don't know what they are showing. Every graph needs to include a label next to the numberline

*After* the numberline(s) and labels are created, you can fit your data onto the numberline to create the graph.

In the next few sections, we are going to look at a few different types of graphs and what types of variables they are useful for. The following table is an illustration the different types of graphs we will see and what variable types they are good for.

| Quantitative Graphs  | Categorical Graphs |
| :------------------: | :----------------: |
| Dotplot              | Bar graph          |
| Stem-and-leaf plot   | (Paretto chart)    |
| Box-and-whisker plot | Pie chart          |
| Scatterplot          |                    |
| Timeseries           |                    |
| Histogram ---------> | Histogram          |

A *histogram* takes quantitative data and categorizes it. Once categorized, you make a bar graph. The histogram will be the subject of lesson 5.

The box-and-whisker plot (commonly known as the boxplot) will be discussed in lesson 6.