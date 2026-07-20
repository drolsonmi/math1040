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
<title>Solution for practice 13.1.3</title>
</head>

## 13.1 What is a Binomial Distribution? - Solution for Practice 3
3. Historically, 8% of emails sent by a marketing company are marked as spam by the recipient's inbox. The company sends a new campaign to 500 independent recipients, and we count how many mark it as spam.

### Solution

Check the four requirements:
- Fixed number of trials: yes, $n=500$ emails.
- Two outcomes: yes, each email is either marked as spam (success) or not (failure).
- Constant probability: yes, each recipient has the same 8% historical probability of marking the email as spam.
- Independent trials: yes, the problem tells us the recipients are independent, so one person's action doesn't affect another's.

All four requirements are met, so this **is a binomial experiment**.

$$n = 500 \qquad p = 0.08 \qquad q = 1-0.08 = 0.92$$

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_1_WhatIsBinomial.html#practice)
