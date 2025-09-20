<head>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
</head>

## Practice Question 11.1.3
If you have a secure password, then it is very difficult for a hacker to randomly guess your password. Is it safer to have an 8-character password that can contain any character \{a-z, A-Z, 0-9, !@#$%^&*() \} or a 12-character password with only lower-case letters? 

Take a second and make a guess as to which is more secure. Then use the Fundamental Counting Rule to find the number of possible 8-character and 12-character passwords. The option with more possible passwords would be more secure as it is more difficult to randomly guess.

### Answer to Practice Question 11.1.3
For the 8-character complex password, there are 26 letters (lower- and upper-case), 10 digits, and 10 special characters. That is a total of 72 different characters. Each character of the password can be any of the 72 characters, so the number of different possible passwords is,

$$\begin{align*}
  72 * 72 * 72 * 72 * 72 * 72 * 72 * 72 &= 72^8 \\
    &= 7.222*10^{14} \\
    &= 722,200,000,000,000 (722.2 trillion)
\end{align*}$$

For the 12-character simple password, there are only 26 different possible characters. Each character can be any of the 26 characters, so the number of different possible passwords is,

$$\begin{align*}
  26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 * 26 &= 26^12 \\
  &= 9.543*10^{16} \\
  &= 95,430,000,000,000,000 (95.4 quadrillion)
\end{align*}$$

Since there are more possible passwords for the 12-character simple password, this would be more secure password.

*Note*: Of course, length combined with complexity is a better option, so the more secure option would be a 12-character password with any character \{a-z, A-Z, 0-9, !@#$%^&*() \}. Passphrases that are 15-30 characters long are even more secure. However, these options weren't addressed in the question.