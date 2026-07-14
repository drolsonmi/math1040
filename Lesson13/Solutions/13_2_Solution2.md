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
2. A multiple-choice quiz has 10 questions, each with 4 answer choices. A student guesses randomly on every question. What is the probability that the student gets exactly 3 questions correct?

### Solution

**Step 1: Check that this is a binomial experiment, and identify $n$, $p$, and $k$.**

There is a fixed number of trials (10 questions), each question has two outcomes (correct/incorrect), the probability of guessing correctly is the same on every question, and the questions are independent of each other. This is a binomial experiment.

- $n = 10$
- $p = \frac{1}{4} = 0.25$ (probability of guessing correctly out of 4 choices)
- $k = 3$

**Step 2: Set up the binomial probability formula.**

$$P(X=3) = \binom{10}{3}(0.25)^3(0.75)^7$$

**Step 3: Calculate the combination.**

$$\binom{10}{3} = \frac{10!}{3!\,7!} = 120$$

**Step 4: Calculate the powers and multiply.**

$$(0.25)^3 = 0.015625 \qquad (0.75)^7 \approx 0.13348$$

$$P(X=3) = 120 \times 0.015625 \times 0.13348 \approx 0.2503$$

There is about a **25.0% chance** that the student gets exactly 3 questions correct by random guessing.

[Return to lesson](https://drolsonmi.github.io/math1040/Lesson13/13_2_BinomialProbabilities.html#practice)
