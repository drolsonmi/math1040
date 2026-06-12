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
<title>3.2 Experimental Studies</title>
</head>

# Lesson 3.2 Experimental Studies
## Reading
Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)
* 1.5.1 Experimental Studies, Control/Treatment groups, Placebos (pages 30-31)

## Lesson
Observational studies are used when we look at the current (or rather, uninfluenced) state of our sample. There are times, however, when we do want to influence the outcome. For example, if we want to determine whether one condition will affect the outcome or not, we create an experiment to test it. 

Here is an example of the difference between Observational and Experimental studies. 
- __Observational Study__: Is there an association between a student's daily self-reported caffeine consumption and their performance on a standardized short-term memory test?
  - *To implement*: Collect data on each students daily caffeine intake and test results
- __Experimental Study__: Does caffeine intake increase or decrease short-term memory test performance?
  - *To implement*: Separate their sample into two groups
    - Measure results from group 1, not allowing them to take caffeine 
    - Measure results from group 2, allowing them to take caffeine
    - Compare results between the two groups, seeing if there is an increase or decrease in performance with caffeine intake

### Control and Treatment Groups
In an experimental study, we divide our sample into two groups. 

One group remains unaffected from our study. With this group, we simply observe them. This is known as a __control group__.

To test the experiment, we take the other group and introduce our new variable (the variable we are using to test our experiment, also known as the __treatment variable__). The group introduced to the treatment variable is known as a __treatment group__.

### Sampling an Experimental study
There are a few different methods to divide our sample into control and treatment groups.

In a __completely randomized experiment__, subjects in the experiment are randomly separated into control and treatment groups. The treatment group is given the treatment variable, but the control group is tested without the treatment variable.

A __blocked experiment__ separates the sample into groups by similar variables (similar to a stratified sample). Each group is then randomly selected into two subgroups, the control group and treatment group. Then we can examine how the treatment variable affects different groups.

In a __matched pair experiment__, subjects are separated into groups matching as many confounding variables as possible. That way, the two subjects are as identical as possible. Then one of the subjects is selected for the treatment group and the other remains in the control group.


<iframe width="560" height="315" src="https://www.youtube.com/embed/mmn_RhZO6vs?si=9xbZUVcXsHOklf5S" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Summary
* __Observational Study__: Studies where data are collected only by monitoring what occurs
* __Experimental Study__: Studies where yours sample is introduced to a new variable to be tested
  * __Control Group__: The portion of the sample that is unaffected by the tested variable
  * __Treatment Group__: The portion of the sample that is affected by the tested variable
* __Completely randomized experiment__: Subjects are randomly assigned to each group in the experiment
* __Blocked experiment__: Subjects grouped based on the identified variable
  * Randomize subjects within each group as control or treatment
* __Matched pairs experiment__: Pairs of people are matched on as many variables as possible, so that the comparison happens between very similar cases. One is made a control, the other treatment.

## Practice
Here are some scenarios of possible experimental studies to design. For each scenario, describe each of the following:
- Treatment variable
- Subjects in the control group
- Subjects in the treatment group
- Explanatory and response variables

1. A pharmaceutical company wants to test whether a new pain reliever reduces headache symptoms faster than a standard over-the-counter drug. They randomly assign 200 headache patients to receive either the new drug or the existing drug, then measure how many minutes it takes for symptoms to subside.
    * [After solving on your own, check the solution](./Solutions/3_2_Solution1.html)

2. An agricultural researcher wants to know if a new fertilizer increases corn yield. They randomly assign 30 plots of farmland to receive either the new fertilizer or no fertilizer, then measure the bushels of corn harvested per acre at the end of the season.
    * [After solving on your own, check the solution](./Solutions/3_2_Solution2.html)

3. A school district wants to test whether a new reading curriculum improves student test scores. They select 6 elementary schools and randomly assign 3 schools to use the new curriculum and 3 schools to use the existing curriculum. At the end of the year, they compare average reading scores across the two groups.
    * [After solving on your own, check the solution](./Solutions/3_2_Solution3.html)
