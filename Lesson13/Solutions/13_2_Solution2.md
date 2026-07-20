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
<title>Solution for practice 13.2.2</title>
</head>

## 13.2 Binomial Probabilities - Solution for Practice 2
2. A multiple-choice quiz has 10 questions, each with 4 answer choices. A student guesses randomly on every question. Find the probability that the student gets exactly 3 questions correct.

### Solution

Since there are 4 choices and the student is guessing, $p = \frac{1}{4} = 0.25$ for each question. Identify the values: $n=10$, $p=0.25$, $q=0.75$, $x=3$.

$$P(3) = \binom{10}{3}(0.25)^3(0.75)^7$$

**Step 1: Find the combination.**

$$\binom{10}{3} = \frac{10!}{3!7!} = 120$$

**Step 2: Find the probability powers.**

$$(0.25)^3 = 0.015625 \qquad (0.75)^7 \approx 0.13348$$

**Step 3: Multiply everything together.**

$$P(3) = 120(0.015625)(0.13348) \approx 0.2503$$

The probability that the student guesses exactly 3 questions correctly is about **25.03%**.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_2_BinomialProbabilities.html#practice)
