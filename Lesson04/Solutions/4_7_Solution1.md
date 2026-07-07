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
<title>Solution for practice 4.7.1</title>
</head>

## 4.7 Timeseries - Solution for Practice 1
 
1. The table below shows the average monthly high temperature (in °F) for a city over one year:
| Month | Jan | Feb | Mar | Apr | May | Jun | Jul | Aug | Sep | Oct | Nov | Dec |
| ----- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Temp  | 32  | 36  | 45  | 58  | 68  | 78  | 84  | 82  | 74  | 60  | 46  | 34  |
 
  - Create a timeseries graph of this data, including a proper scale, labels, and title.
  - Describe any trend or seasonality you observe.
  
### Solution
 
Since time (Month) is always the explanatory variable, it goes on the x-axis. Average High Temperature is the response variable and goes on the y-axis. Plot a point for each month and connect them in order with line segments:
 
![Timeseries graph of average monthly high temperature](https://drolsonmi.github.io/math1040/Lesson04/images/Fig471_Solution.png)
 
**Trend/seasonality**: This graph shows clear **seasonality** rather than a long-term trend — temperatures rise from January through July, peak in the summer, and then fall back down through the end of the year. This up-and-down pattern would repeat again the following year, which is the hallmark of a seasonal pattern rather than an overall upward or downward trend.
 
Be sure that your graph includes:
 
- proper scales
- proper labels
- a title
[Return to lesson](https://drolsonmi.github.io/math1040/Lesson04/4_7_Timeseries.html#practice)