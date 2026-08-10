<head>
<title>24.1 Reminder of Dependent Samples & the Difference Variable</title>
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

# Lesson 24.1 Dependent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.1 Paired data (page 209)

## Lesson

### A Reminder: What Makes Samples Dependent?
Back in Lesson 22.1, we said two samples are **dependent (paired)** when each individual or item in one sample is naturally matched with exactly one individual or item in the other sample — most commonly because the *same* individuals were measured twice (before/after, pretest/posttest, left hand/right hand).

Lesson 22 dealt with **independent** samples, where we needed brand-new formulas involving two separate means, $\bar{x}_1$ and $\bar{x}_2$. Dependent samples let us do something much simpler.

### The Key Idea: Build a Difference Variable
Because each pair belongs to the same individual, we can subtract the two measurements for every individual and get a single new number for each person:

$$d = x_1 - x_2$$

Instead of two separate lists of numbers, we now have **one** list — the list of differences. This is the entire trick of this lesson: **a paired two-sample problem is secretly a one-sample problem**, just like the ones we solved back in Lessons 18 and 20. We are simply going to run a one-sample t-test on $d$, using a null value of 0 (since $H_0$ will always claim there's no difference).

> __Important:__ Be consistent about the order of subtraction ($x_1 - x_2$ or $x_2 - x_1$) for every pair, and keep track of which order you used — it determines whether a positive $\bar{d}$ means group 1 is larger or group 2 is larger. We'll return to this in Lesson 24.2.

### Finding $\bar{d}$ and $s_d$
Once we have our list of differences, we treat it exactly like any other quantitative dataset:

$$\bar{d} = \frac{\sum d}{n} \qquad\qquad s_d = \sqrt{\frac{\sum(d-\bar{d})^2}{n-1}}$$

Here, $n$ is the number of **pairs** (not the total number of measurements).

### Example

> A clinic wants to know whether a new medication lowers systolic blood pressure. Blood pressure is measured for 10 patients before starting the medication, and again after 4 weeks on the medication.

| Patient | Before ($x_1$) | After ($x_2$) | Difference ($d = x_1-x_2$) |
| :-----: | :------------: | :-----------: | :------------------------: |
| 1       | 148            | 140           | 8                          |
| 2       | 152            | 145           | 7                          |
| 3       | 139            | 138           | 1                          |
| 4       | 160            | 150           | 10                         |
| 5       | 145            | 138           | 7                          |
| 6       | 155            | 148           | 7                          |
| 7       | 150            | 144           | 6                          |
| 8       | 142            | 139           | 3                          |
| 9       | 158            | 150           | 8                          |
| 10      | 149            | 141           | 8                          |

Since the same 10 patients were measured twice, this is a **dependent (paired) sample**, and we subtract Before − After for each patient.

**Finding $\bar{d}$:**

$$\bar{d} = \frac{8+7+1+10+7+7+6+3+8+8}{10} = \frac{65}{10} = 6.5$$

**Finding $s_d$:**

| $d$   | $d - \bar{d}$ | $(d-\bar{d})^2$ |
| :---: | :-----------: | :-------------: |
| 8     | 1.5           | 2.25            |
| 7     | 0.5           | 0.25            |
| 1     | -5.5          | 30.25           |
| 10    | 3.5           | 12.25           |
| 7     | 0.5           | 0.25            |
| 7     | 0.5           | 0.25            |
| 6     | -0.5          | 0.25            |
| 3     | -3.5          | 12.25           |
| 8     | 1.5           | 2.25            |
| 8     | 1.5           | 2.25            |

$$\sum(d-\bar{d})^2 = 64.5 \qquad\qquad s_d = \sqrt{\frac{64.5}{9}} \approx 2.677$$

We now have everything we need to run a one-sample t-test on the differences: $\bar{d} = 6.5$, $s_d \approx 2.677$, $n = 10$. We'll use these values throughout the rest of this lesson.

## Practice
For each dataset, identify the paired differences, then find $\bar{d}$ and $s_d$.

1. A researcher tests whether caffeine improves reaction time (in milliseconds). Reaction time is measured for 5 participants before and after drinking a cup of coffee.

    | Participant | Before | After |
    | :---------: | :----: | :---: |
    | 1           | 320    | 290   |
    | 2           | 305    | 295   |
    | 3           | 310    | 300   |
    | 4           | 298    | 285   |
    | 5           | 315    | 292   |

    Find $\bar{d}$ and $s_d$ using $d = \text{Before} - \text{After}$.
    * [After solving on your own, see solution here](./Solutions/24_1_Solution1.md)

2. An instructor wants to know if a review session improves exam scores. 6 students take a pretest, attend the review session, then take a posttest.

    | Student | Pretest | Posttest |
    | :-----: | :-----: | :------: |
    | 1       | 62      | 68       |
    | 2       | 70      | 74       |
    | 3       | 58      | 65       |
    | 4       | 75      | 78       |
    | 5       | 66      | 70       |
    | 6       | 80      | 79       |

    Find $\bar{d}$ and $s_d$ using $d = \text{Posttest} - \text{Pretest}$.
    * [After solving on your own, see solution here](./Solutions/24_1_Solution2.md)

3. A nutritionist tracks the weight (in lbs) of 5 participants before and after a 6-week diet program.

    | Participant | Before | After |
    | :---------: | :----: | :---: |
    | 1           | 210    | 202   |
    | 2           | 185    | 180   |
    | 3           | 232    | 225   |
    | 4           | 198    | 190   |
    | 5           | 205    | 200   |

    Find $\bar{d}$ and $s_d$ using $d = \text{Before} - \text{After}$.
    * [After solving on your own, see solution here](./Solutions/24_1_Solution3.md)
