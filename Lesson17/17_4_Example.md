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
</head>

# Lesson 17.4 Example using the Central Limit Theorem
Here is a full example of how we use the Central Limit Theorem. We'll first look at a probability calculation for a single event, then we'll look at a number of samples. Here's what you'll see:
* The probability of a single outlier is low, but still possible
* The probability of an entire sample being made of outliers is extemely low
    * That is, the average of a sample has a higher probability of being closer to the mean

Here is the scenario that we will work with:

> A company makes generic, low-cost ink cartridges for printers. They claim that the average number of copies a cartridge will produce is 1000 copies with a standard deviation of 120 copies. The number of copies a cartridge makes follows a normal distribution.​

I am going to ask you to calculate the probability that a single cartridge prints fewer than 800 copies. Then I'll ask you to calculatoe the probability that the average of 5 randomly selected cartridges is fewer than 800.

Let's think about this logically before we do it mathematically. If I get one cartridge that prints fewer than 800 cartridges, is that unusual? Perhaps it is unusual, but not really cause for alarm. I would expect that every once in a while there is a printer cartridge that doesn't perform to expectation. It happens.

But if I randomly select 5, what are the chances that the average printing performance is less than 800 copies? If the company claims that their average is 1000, then a random selection's average should definitely not be less than 800. If that happens, that would definitely be unusual and cause for alarm.

So, I would expect from my calculations that a single cartridge would have a small but possible probability, while my sample will show an extremely small probability.

Now, let's find out.

### Single Event
Let's start with a single event. Let's answer this question:

> Find the probability that a single cartridge chosen at random will print no more than 800 copies

So, we want to know the probability that we have a cartridge that prints fewer than 800 copies. That is, $P(x < 800)$. We'll start by finding the z-score.

$$z = \frac{x-\mu}{\sigma} = \frac{800-1000}{120} = \frac{-200}{120} = -1.67$$

Now, we look at a z-table and find -1.67 on the z-table. We find that,

$$P(x < 800) = P(z < -1.67) = 0.0475 = 4.75\%$$

There is a 4.75% chance that we randomly select a __single__ cartridge that will print no more than 800 copies.

### Sample of events
Now, let's try work with a random sample of 5 cartridges. In order to do this, *we must make sure that the Central Limit Theorem applies*. Let's restate the problem, then check the two conditions for the central limit theorem.

> A company makes generic, low-cost ink cartridges for printers. They claim that the average number of copies a cartridge will produce is 1000 copies with a standard deviation of 120 copies. The number of copies a cartridge makes follows a normal distribution.​

Do you remember the two conditions?
* __Is the sample randomly selected?__
    * In the problem, it specifically states that the sample is random, so yes, this condition is satisfied.
* __Is the sample large enough?__
    * Since this is a quantitative sample, we need $n > 30$. Our sample size is only 5, so it is not large enough.
    * However, remember that there is an exception if our population is normally distribution. Look at the problem, and you'll see that it is. So, we have satisfied this condition.

Since we satisfied both conditions, the central limit theorem applies and we can continue.

We are now working with a sample. So, let's find our sampling mean and sampling standard deviation.

$$\mu_\bar{x} = \mu = 1000 \qquad \sigma_\bar{x} = \frac{\sigma}{\sqrt{n}} = \frac{120}{\sqrt{5}} = \frac{120}{2.2360} = 53.67$$

Now, we can find our z-score with our new mean and standard deviation for our sample.

$$z = \frac{\bar{x} - \mu_\bar{x}}{\sigma_\bar{x}} = \frac{800 - 1000}{53.67} = \frac{-120}{53.67} = -3.73$$

We can now look up this probability. (This z-score actually won't be on a z-table. That means it's going to be really small! We'll have to use a calculator for this one.)

$$P(\bar{x} < 800) = P(z < -3.73) = 0.000097 = 0.0097\%$$

So, the probability that a single individual cartridge printing fewer than 800 copies is 4.75%. On the other hand, the probability that the average of 5 random cartridges is 0.0097%. This is exactly what we expected before we started our calculations.