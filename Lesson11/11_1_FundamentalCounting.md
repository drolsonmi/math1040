<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

# Lesson 11.1 Fundamental Counting Rule
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 7.1.1 ---

## Lesson
We have discussed the probabilities of a single event (lessons 9-10). But what if you have multiple events at the same time? For example, we roll not one die but two dice. Or instead of choosing marbles from 5 different bags. Or choosing toppings for a pizza (choosing meats, cheese, and toppings). All of these have multiple events. In this lesson, we will learn how to calculate the probabilities of multiple events.

Consider two dice - one 4-sided white die and one 6-sided black die. If the white die rolls a 3, we'll call that `W3`, and if the black die rolls a 5, we'll call that `B5`. Now, roll the dice. How many possibilities are there?
* If we roll `W1`, there are 6 possibilities for black: (`W1,B1`),(`W1,B2`),(`W1,B3`),(`W1,B4`),(`W1,B5`),(`W1,B6`)
* If we roll `W2`, there are 6 possibilities for black: (`W2,B1`),(`W2,B2`),(`W2,B3`),(`W2,B4`),(`W2,B5`),(`W2,B6`)
* If we roll `W3`, there are 6 possibilities for black: (`W3,B1`),(`W3,B2`),(`W3,B3`),(`W3,B4`),(`W3,B5`),(`W3,B6`)
* If we roll `W4`, there are 6 possibilities for black: (`W4,B1`),(`W4,B2`),(`W4,B3`),(`W4,B4`),(`W4,B5`),(`W4,B6`)
* *Bottom line*: There are 4 possibilities for the white die. For each possibility, there are 6 possibilities for the black die. That is a total of $$4\times 6 = 24$$ possibilities

That's it! That is the __Fundamental Counting Rule__. 
> If event A has $$k$$ different possibilities, and event B has $$n$$ different possibilities, then __the total number of combined possibilities is $$k\times n$$__.

What about 3 events? Let's take the 4-sided white die and the 6-sided black die, and we'll add a 10-sided red die.
* There are 24 possibilities with the white and black dice
* For each possibility with the white and black dice, there are 10 possibilities for the red die
* That's a total of $$24\times 10 = 240$$ possible combinations

The complete __Fundamental Counting Rule__.
> For multiple events, let's say that event $$i$$ has $$n_i$$ different possible outcomes. __The total possible combinations is, $$n_1 \times n_2 \times n_3 \times \dots$$__.

<iframe width="560" height="315" src="https://www.youtube.com/embed/3inwc2NFqJ4?si=Ik0LIDb6bBihT-oL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/jqxmWx5lGIU?si=nBhEm1bdL-zT2r1M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
Here are three example problems using the Fundamental Counting Rule. Answer the questions to the best of your ability then *afterwards* check the answer.

### Practice Problem 11.1.1
Papa Miguel's pizza place allows you to choose your sauce, cheese and 1 topping for a flat price. The menu has the following options:
* Sauce: Tomato, BBQ, Alfredo
* Cheese: Mozerella, 5-cheese, Mexican, Parmesan
* Toppings: Pepperoni, Sausage, Chicken, Ham, Bacon, Pineapple, Onion, Taco Beef

How many possible pizza combinations could you create?

* After solving on your own, [check the solution](Solutions/11_1_Solution1.md).

### Practice Problem 11.1.2
There are 13 people in a race. How many ways can the 13 runners cross the finish line?

* After solving on your own, [check the solution](Solutions/11_1_Solution2.md).

### Practice Problem 11.1.3
If you have a secure password, then it is very difficult for a hacker to randomly guess your password. Is it safer to have an 8-character password that can contain any character \{a-z, A-Z, 0-9, !@#$%^&*() \} or a 12-character password with only lower-case letters? 

Take a second and make a guess as to which is more secure. Then use the Fundamental Counting Rule to find the number of possible 8-character and 12-character passwords. The option with more possible passwords would be more secure as it is more difficult to randomly guess.

* After solving on your own, [check the solution](Solutions/11_1_Solution3.md).

<!--
## Technology

### TI-83/84

### Excel

### Desmos
-->