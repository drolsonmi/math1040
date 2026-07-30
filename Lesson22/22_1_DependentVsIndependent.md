<head>
<title>22.1 Reminder of Dependent vs. Independent Samples</title>
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

# Lesson 22.1 Reminder of Dependent vs. Independent Samples
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 5.4.1 Paired data (page 209)

## Lesson
Before we can compare two samples, we need to know **how** they are related to each other. This determines which formulas we use, so it's worth pausing to review the difference.

### Independent Samples
Two samples are **independent** when the individuals in one sample have no natural relationship to the individuals in the other sample. The two groups are made up of different individuals, selected separately.

*Examples:*
* Comparing the average test scores of students at School A vs. students at School B
* Comparing the average weight loss of people using Diet Plan 1 vs. people using Diet Plan 2 (different people in each group)
* Comparing average commute times for drivers on Route 1 vs. drivers on Route 2

### Dependent (Paired) Samples
Two samples are **dependent**, or **paired**, when each individual (or item) in one sample is naturally matched with exactly one individual (or item) in the other sample. This usually happens when:
* The same individuals are measured twice (e.g., before and after a treatment)
* Individuals are matched in pairs based on shared characteristics (e.g., twins, or left hand vs. right hand of the same person)

*Examples:*
* Comparing each patient's blood pressure before and after taking a new medication
* Comparing an athlete's 40-yard dash time before and after a training program
* Comparing test scores for the same students on a pretest and a posttest

### Why does it matter?
The formulas for confidence intervals and hypothesis tests are different for dependent and independent samples. When samples are paired, we can subtract each pair to get a single new variable (the differences), and then run a **one-sample** test on those differences. When samples are independent, we cannot pair the data this way, so we need formulas that work directly with two separate means (or proportions).

This lesson (Lesson 22) and the next (Lesson 23) focus entirely on **independent** samples. Correctly identifying whether two samples are independent or dependent is always the first step before choosing a method.

## Practice
For each scenario, decide whether the two samples are **dependent** or **independent**, and briefly explain why.

1. A gym wants to know if members' resting heart rate decreases after 8 weeks of a new training program. They measure the same 30 members' resting heart rate before the program begins and again after 8 weeks.
    * [After solving on your own, see solution here](./Solutions/22_1_Solution1.md)
2. A researcher wants to compare average scores on a standardized test between students who attend public school and students who attend private school. She collects scores from 50 randomly selected public school students and 50 different randomly selected private school students.
    * [After solving on your own, see solution here](./Solutions/22_1_Solution2.md)
3. A sports scientist measures the reaction time of 20 athletes using their dominant hand and then measures the same 20 athletes' reaction time using their non-dominant hand.
    * [After solving on your own, see solution here](./Solutions/22_1_Solution3.md)
