<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<title>Lesson 1.2 Variables</title>
</head>

# Lesson 1.2 Variables
## Reading
Reading selections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 1.2.1 Observations, variables, and data matrices (pages 11-12)
* 1.2.2 Types of Variables (pages 12-13)
* 1.2.3 Relationships between variables (pages 13-15)

## Lesson
All variables can be identified as one of two types:
* __Quantitative__ (or numerical) variables deal with numbers. We can do mathematical calculations on these.
* __Categorical__ (or qualitative) variables deal with groups. Doing math on these variables will not make sense. Instead, we count the occurrences in each category and deal with percentages and probabilities.

<table style="margin: 1.2em 0px; padding: 0px; border-collapse: collapse; border-spacing: 0px; font: inherit; border: 0px;">
                <thead>
                    <tr style="border-width: 1px 0px 0px; background-color: white; margin: 0px; padding: 0px; border-color: #cccccc initial initial initial; border-style: solid initial initial initial;">
                        <th style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; background-color: #f0f0f0;">Quantitative (or Numerical)</th>
                        <th style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; background-color: #f0f0f0;">Qualitative (or Categorical)</th>
                    </tr>
                </thead>
                <tbody style="margin: 0px; padding: 0px; border: 0px;">
                    <tr class="" style="border-width: 1px 0px 0px; background-color: white; margin: 0px; padding: 0px; border-color: #cccccc initial initial initial; border-style: solid initial initial initial;">
                        <td class="" style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; vertical-align: top;">
                            <p>Deals with numbers</p>
                            <ul>
                                <li>Can take an average, and the average has meaning</li>
                                <li>Can do other mathematics</li>
                            </ul>
                        </td>
                        <td style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em; vertical-align: top;">
                            <p>Deals with categories</p>
                            <ul>
                                <li>Words</li>
                                <li>Levels</li>
                                <li>Identification
                                    <ul>
                                        <li>Can be numbers, but an average is meaningless</li>
                                    </ul>
                                </li>
                            </ul>
                        </td>
                    </tr>
                    <tr style="border-width: 1px 0px 0px; background-color: #f8f8f8; margin: 0px; padding: 0px; border-color: #cccccc initial initial initial; border-style: solid initial initial initial;">
                        <td style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em;">
                            <p>Examples:</p>
                            <ul>
                                <li>GPA</li>
                                <li>Age</li>
                                <li>Weight</li>
                                <li>Height</li>
                                <li>Number of pets</li>
                                <li>Distances</li>
                                <li>Time (elapsed time: 25 seconds, 5 months, 42 years)</li>
                            </ul>
                        </td>
                        <td style="font-size: 1em; border: 1px solid #cccccc; margin: 0px; padding: 0.5em 1em;">
                            <p>Examples:</p>
                            <ul>
                                <li>Favorite ice cream flavor (Vanilla, Chocolate, Strawberry)</li>
                                <li>Grade Level (Freshman, Sophomore, Junior, Senior)</li>
                                <li>Grade Level (9, 10, 11, 12, 13+)</li>
                                <li>Phone number</li>
                                <li>ZIP Code</li>
                                <li>Student ID</li>
                                <li>Date (referenced time: January, 6th century, 2024)&nbsp;</li>
                            </ul>
                        </td>
                    </tr>
                </tbody>
            </table>

<iframe width="560" height="315" src="https://www.youtube.com/embed/sNPDOEc3a6w?si=39XQuSYhtot8ZWZh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Examples
You want to collect data on the cell phone networks most commonly used among Snow College students. You collect *the network names* from 100 students. What type of variable is this?
  * Possible answers include {"Verizon Wireless", "AT&T", "T-Mobile", "Boost Mobile", "Cricket", ...}. These are just words, so math cannot be done on them
  * The students are categorized (or grouped together) based on their answer to this question
  * So, __this is a categorical variable__.

You want to study our dependence on computers. You ask Snow College students *how many computers are used in their houses*. What type of variable is this?
  * Possible answers are a number {1, 2, 3, 4, ...}. The context of the question indicates that we do want to consider these as numbers, and doing math makes sense (such as taking an average number of computers in a house)
      * *Note:*Although you could use the number of computers to categorize the students (such as "0-2 computers", "3-5 computers", "More than 5"), the context of the question indicates that we want to focus on the numerical aspect of this variable
  * So, __this is a quantitative variable__.

What regions of Utah are most represented by Snow College students? You ask students for their *ZIP codes*. What type of variable is this?
  * Possible answers are 5-digit numbers, such as {84102, 84109, 84627, 84642, 84698, ...}
  * Even though they are numbers, we aren't focusing on the number. They are only used to group students into regions
    * The average ZIP code doesn't make sense
  * So, even though the answers are numbers, __this is a categorical variable__.

## Practice
Here are a few variables. Determine if they are Quantitative or Categorical.
1. Age
    * [After solving on your own, see solution here](Solutions/1_2_Solution1.md)
2. Eye color
    * [After solving on your own, see solution here](Solutions/1_2_Solution2.md)
3. Value of a house
    * [After solving on your own, see solution here](Solutions/1_2_Solution3.md)
4. GPA
    * [After solving on your own, see solution here](Solutions/1_2_Solution4.md)
5. Pain Level (No pain, Little pain, Moderate pain, Strong pain, Intense pain)
    * [After solving on your own, see solution here](Solutions/1_2_Solution5.md)
6. Phone number
    * [After solving on your own, see solution here](Solutions/1_2_Solution6.md)


