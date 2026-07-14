<head>
<title>Lesson 12.1 Probability Distributions</title>
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

# Lesson 12.1 Probability Distributions
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)

## Probability Distribution
The core of all distributions is the __probability distribution__. A probability distribution simply describes the frequency of times each possible outcome of a given event occurs. For example, here is a distribution showing how many people in each age group attended an event:

| Age       | 0-4   | 5-9   | 10-14 | 15-19 | 20-24 | 25-29 | 30-34 |
| :-------- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Count     | 10    | 15    | 12    | 25    | 29    | 32    | 23    |
| Frequency | 0.068 | 0.103 | 0.082 | 0.171 | 0.199 | 0.219 | 0.158 |

This shows how all subjects in our sample are distributed through all categories.

There are two very important rules for probability distributions:
1. Each probability has to be between 0 and 1
2. All probabilities have to add up to 1

If one of these rules is broken, then we have an invalid probability distribution.

<iframe width="560" height="315" src="https://www.youtube.com/embed/bbliECmvm94?si=NNWuwfASrpChY7MB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice
1. Here is a probability distribution with one missing value. Determine what that value should be.

    | Category    |   A   |   B   |   C   |   D   |   E   |   F   |
    | :---------- | :---: | :---: | :---: | :---: | :---: | :---: |
    | Probability | 0.08  | 0.16  | 0.22  | 0.34  | 0.18  |   x   |

  - [After solving on your own, see solution here](Solutions/12_1_Solution1.md).

2. Here are three distributions. One of them is invalid. Determine which is the invalid distribution and what can be done to fix it.

    | Distribution 1 |   A   |   B   |   C   |   D   |   E   |   F   |
    | :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
    | Probability    | 0.05  | 0.12  | 0.15  | 0.18  | 0.23  | 0.27  |

    | Distribution 2 |   A   |   B   |   C   |   D   |   E   |   F   |
    | :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
    | Probability    | 0.14  | 0.20  | 0.24  | 0.22  | 0.14  | 0.09  |

    | Distribution 3 |   A   |   B   |   C   |   D   |   E   |   F   |
    | :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
    | Probability    | 0.17  | 0.17  | 0.16  | 0.16  | 0.17  | 0.17  |

  - [After solving on your own, see solution here](Solutions/12_1_Solution2.md).

3. Here are three distributions. One of them is invalid. Determine which is the invalid distribution and what can be done to fix it.

    | Distribution 1 |   A   |   B   |   C   |   D   |   E   |   F   |
    | :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
    | Probability    | 0.24  | 0.28  | 0.24  | 0.19  | -0.11 | 0.16  |

    | Distribution 2 |   A   |   B   |   C   |   D   |   E   |   F   |
    | :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
    | Probability    | 0.04  | 0.09  | 0.13  | 0.16  | 0.26  | 0.32  |

    | Distribution 3 |   A   |   B   |   C   |   D   |   E   |   F   |
    | :------------- | :---: | :---: | :---: | :---: | :---: | :---: |
    | Probability    | 0.13  | 0.17  | 0.24  | 0.21  | 0.16  | 0.09  |

  - [After solving on your own, see solution here](Solutions/12_1_Solution3.md).

<!--
## Technology

### TI-83/84

### Excel

### Desmos
-->
