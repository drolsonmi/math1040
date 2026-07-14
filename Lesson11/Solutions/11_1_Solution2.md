<head>
<title>Solution for practice 11.1.2</title>
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

## 11.1 Fundamental Counting Rule - Solution for Practice 2
There are 13 people in a race. How many ways can the 13 runners cross the finish line?

### Answer to Practice Question 11.1.2
* There are 13 different contestants who can place 1st.
* There are 12 different contestants who can place 2nd (all but the 1st place contestant).
* There are 11 different contestants who can place 3rd (all but the 1st and 2nd place contestants).
* There are 10 different contestants who can place 4th (all but the 1st, 2nd, and 3rd place contestants).
* There are 9 different contestants who can place 5th (all but the 1st, 2nd, 3rd, and 4th place contestants).
* There are 8 different contestants who can place 6th (all but the 1st - 5th place contestants).
* There are 7 different contestants who can place 7th (all but the 1st - 6th place contestants).
* There are 6 different contestants who can place 8th (all but the 1st - 7th place contestants).
* There are 5 different contestants who can place 9th (all but the 1st - 8th place contestants).
* There are 4 different contestants who can place 10th (the last 4 runners).
* There are 3 different contestants who can place 11th (the last 3 runners).
* There are 2 different contestants who can place 12th (the last 2 runners).
* There is only 1 contestant who can place 13th (the last runner).

Using the Fundamental Counting Rule, there are 

$$13\times 12\times 10\times 9\times 8\times 7\times 6\times 5\times 4\times 3\times 2\times 1 = \mathbf{6,227,020,800}$$

possible ways the 13 contestants can cross the finish line.
