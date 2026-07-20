<head>
<title>Lesson 15.4 Finding Z-scores from a Probability</title>
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

# Lesson 15.4 Finding Z-scores from a Probability
## Reading

Reading sections are from the [Introductory Statistics Textbook](../Resources/OpenIntroTextbook.pdf)

- 4.1.5 Calculator: finding normal probabilities (pages 148-150)

## Lesson

<iframe width="560" height="315" src="https://www.youtube.com/embed/RxKY0Hf5G5k?si=aaMtuhgHnZWqbf6e" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

So far, we've started with a value (or a z-score) and worked forward to find a probability. In this lesson, we'll work in the **opposite direction**: starting with a probability (or percentile) and working backward to find the z-score, and then the actual data value, that produces it.

This is useful anytime a question describes a *percentage or percentile* rather than a specific value — for example, "what score marks the top 10% of test-takers?" or "what weight separates the lightest 25% of packages from the rest?"

### Step 1: Find the z-score

Instead of looking a z-score up on the *outside* of the Z-table and reading a probability from the *inside*, we do the reverse: we look for the given probability (area to the left) *inside* the table, and read the z-score off the outside edges. Many calculators and spreadsheet programs have a built-in function (often called `invNorm` or `NORM.INV`) that does this instantly — see the Technology section below.

### Step 2: Convert the z-score to a data value

Once we have the z-score, we use the rearranged z-score formula to solve for the actual value $x$:

$$z=\frac{x-\mu}{\sigma} \qquad \Longrightarrow \qquad x=\mu+z\cdot\sigma$$

This two-step process — find the z-score, then convert it to $x$ — is the reverse of everything we did in Lesson 15.3, and it's the key tool for answering percentile and quartile questions, which we'll practice extensively in Lesson 16.

## Technology

### TI-83/84

<iframe width="560" height="315" src="https://www.youtube.com/embed/8hCPrf3AUdU?si=wJlxhAiEiFQcaxzs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Excel

<iframe width="560" height="315" src="https://www.youtube.com/embed/_xXdGU60Y48?si=8KnQEujYlv7EP1mD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Desmos

<iframe width="560" height="315" src="https://www.youtube.com/embed/sMEoedv3MVA?si=roeXU-BnnGHuC02q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Practice

1. SAT Math scores are approximately normally distributed with $\mu = 500$ and $\sigma = 100$. Find the score that marks the **90th percentile** (the score with 90% of test-takers scoring below it).
  - [After solving on your own, see solution here](./Solutions/15_4_Solution1.html)
2. A machine produces metal rods with lengths that are approximately normally distributed with $\mu = 5$ cm and $\sigma = 0.05$ cm. Find the length that separates the shortest **5%** of rods from the rest.
  - [After solving on your own, see solution here](./Solutions/15_4_Solution2.html)
3. Delivery times for a pizza restaurant are approximately normally distributed with $\mu = 45$ minutes and $\sigma = 5$ minutes. Find the two delivery times that bound the **middle 90%** of all deliveries.
  - [After solving on your own, see solution here](./Solutions/15_4_Solution3.html)
