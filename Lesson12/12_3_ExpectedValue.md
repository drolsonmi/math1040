<head>
<title>Lesson 12.3 Expected Value</title>
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

# Lesson 12.3 Expected Value
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 

## Expected Values
With quantitative data, you can find the center by using the mean, the median, and the mode. But how do you calculate the center of categorical data? What is the middle of the categorical set {Exhausted, Tired, Normal, Energized}, taking into account the probabilities of each category?

To calculate the center, we use the __expected value__.

Finding the expected value can only be done if there is an order to the categories. In other words, we are working with an *ordinal* variable.

Calculating the expected value can be done in 4 steps:

1. List the categories in order and assign a value to show that order - we'll call this 
2. Find the probability distribution by calculating the relative frequency (probability) of each category: 
3. Multiply the value $$x$$ by its probability $$P(x)$$
4. Add up all the results

This is the mean! (If you are interested in see that, in fact, [the expected value is the mean, look and my proof](./ExProof.md).) Here's the full equation:

$$E[X] = \mu = \sum x\cdot P(x)$$

This can be applied in cases where you have values for each category. If there are no values, we can assign values. Let me give you two examples, one for each scenario.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Yx_M216sUT0?si=xaJ99NOfpvr05_Va" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Example 1 - Values provided
First, we have an example where values are already given to each category. 

I am involved in a program where I pay $1000 for a class. If I successfully pass the class, I get half of the payment back. If I fail the class, I lose the entire amount.

Putting those into concrete numbers:

* If I pass the class, I pay $1000 - $500 = $500
* If I fail the class, I pay $1000

If 80% of the students pass the class, what is the average amount paid per student?

Start by creating a table:

| Category               | Pass  | Fail  |
| :--------------------- | :---: | :---: |
| Value ($$x$$)          | $500  | $1000 |
| Probability ($$P(x)$$) | 0.80  | 0.20  |

To find the expected value, multiply the values by their probabilities, then add up those results.

| Category               | Pass  | Fail  |
| :--------------------- | :---: | :---: |
| Value ($$x$$)          | $500  | $1000 |
| Probability ($$P(x)$$) | 0.80  | 0.20  |
| $$x\cdot P(x)$$        | $500*0.80 = $400 | $1000*0.20 = $200 |

$$E[x] = $400 + $200 = $600$$

So, the expected value, or the average amount paid per student, is $600.

Does this make sense? Most of the students pass, so they only pay $500. But some do fail, so that will raise the average a little bit, so $600 does make sense.

### Example 2 - No values provided
Now, we'll address a scenario where we don't have values for the categories.

After exercising, I track if I feel tired or energetic. I get the following data:

* Exhausted: 12 times
* Tired:  19 times
* Normal: 16 times
*  Energized: 9 times

These categories have an order, from exhausted on one extreme and energized on the other. So, I'm going to assign 0 to the lowest extreme (exhausted) and 3 to the highest (energized). Now, I have a numerical way of representing each category.

| Category  | Exhausted | Tired | Normal | Energized |
| :-------- | :-------: | :---: | :----: | :-------: |
| Value (x) | 0         | 1     | 2      | 3         |

Now, I add the relative frequencies of each category, and multiply the $$x$$ values by $$P(x)$$:

| Category               | Exhausted     | Tired           | Normal          | Energized       |
| :--------------------- | :-----------: | :-------------: | :-------------: | :-------------: |
| Value ($$x$$)          | 0             | 1               | 2               | 3               |
| Probability ($$P(x)$$) | 12/56 = 0.214 | 19/56 = 0.339   | 16/56 = 0.286   | 9/56 = 0.161    |
| $$x\cdot P(x)$$        | 0*0.214 = 0   | 1*0.339 = 0.339 | 2*0.286 = 0.572 | 3*0.161 = 0.483 |

Adding up those results gives me my expected value.

$$\begin{align*}
E[x] &= 0*0.214 + 1*0.339 + 2*0.286 + 3*0.161 \\
     &= 0 + 0.339 + 0.572 + 0.483 \\
     &= \mathbf{1.394}
\end{align*}$$

Now, what does this number mean? On average, my energy level is at 1.394. That is part way between 1 and 2. But remember that 1 means "Tired" and 2 means "Normal". So, on average, I am somewhere between Tired and Normal, a little closer to Tired.

And there you have it! We have found the average of a categorical variable.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ekspNEd_le0?si=Q_7hfFvqhBuuexbq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/mou0Zb4EhAs?si=rP9dkgQzMbjNWaIc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/IdxqnkzRP5g?si=uCPYfEr4ow7pEjvI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Practice
1. A game costs $5 to play. There is a 30% chance of winning $20 (a net gain of $15 after paying to play), and a 70% chance of winning nothing (a net loss of $5). Find the expected value of playing this game, and explain what it means.
  - [After solving on your own, see solution here](./Solutions/12_3_Solution1.html)
2. A company surveys 100 customers about their satisfaction with a new product, using the categories Very Unsatisfied, Unsatisfied, Neutral, Satisfied, and Very Satisfied:
    | Category | Very Unsatisfied | Unsatisfied | Neutral | Satisfied | Very Satisfied |
    | --- | --- | --- | --- | --- | --- |
    | Count | 5 | 10 | 20 | 40 | 25 |
 
  - Assign a numerical value to each category (0 through 4, in order), find the expected value, and interpret what it means.
  - [After solving on your own, see solution here](./Solutions/12_3_Solution2.html)
3. An insurance company sells a policy for $200 per year. Based on past data, there is a 2% chance a policyholder will file a claim for $5,000 in a given year, and a 98% chance no claim is filed. Find the insurance company's expected payout per policy, and find the company's expected profit per policy.
  - [After solving on your own, see solution here](./Solutions/12_3_Solution3.html)
 

## Technology

The expected value, $E[x] = \sum x\cdot P(x)$, is actually just a weighted mean — so each of these tools calculates it using the same tools you'd use to find a mean, just with the probabilities acting as weights.

### TI-83/84

1. Press **STAT**, then select **1: Edit** to open the list editor.
2. Enter your $x$-values into **L1**, and enter the corresponding probabilities $P(x)$ into **L2**.
3. Press **STAT**, arrow over to **CALC**, and select **1: 1-Var Stats**.
4. When prompted, set the first list to **L1** and the frequency list (**FreqList**) to **L2**, then select **Calculate**.
5. Read $\bar{x}$ from the output — since the probabilities in L2 already add up to 1, this value is exactly the expected value, $E[x]$.

### Microsoft Excel

1. Enter your $x$-values in one column (for example, column A) and the corresponding probabilities $P(x)$ in the adjacent column (column B).
2. Click on an empty cell and enter:

   `=SUMPRODUCT(A1:A5, B1:B5)`

   (Adjust the cell range to match wherever your data is located.)
3. This multiplies each $x$-value by its matching probability and adds up all the results in one step — exactly the expected value formula.

### Desmos

1. Go to [desmos.com/calculator](https://www.desmos.com/calculator).
2. Click on an empty expression line and create a table (click the **+** button and select **table**).
3. Enter your $x$-values in the first column (for example, $x_1$) and your probabilities in the second column (for example, $y_1$).
4. On a new line, type: `total(x_1 * y_1)`
5. Desmos will multiply each $x$-value by its matching probability, element by element, and add up the results — giving you the expected value.