# [MATH 1040 - Introduction to Statistics](https://drolsonmi.github.io/math1040/)

# Lesson 5.2 Creating a Histogram

## Reading

Reading sections are from the [Introductory Statistics Textbook](https://drolsonmi.github.io/math1040/Resources/OpenIntroTextbook.pdf)

- 2.1.3 Histograms (pages 51-54)

## Lesson

[https://www.youtube.com/embed/XUthukqSHvQ?si=-8J5bLrCxCY5Tdc8](https://www.youtube.com/embed/XUthukqSHvQ?si=-8J5bLrCxCY5Tdc8)

Steps for creating a histogram

1. Determine the Range: $~~~Range = Maximum - Minimum$
2. Determine the number of bins
  - Sample Size = *n*
  - How many times do you need to double to reach *n*?
3. Create the bins
  - Bin Size: $~~~Bin~Size = \frac{Range}{n}$
  - Starting point
    * First bin starts at minimum
    * Add the bin size to the minimum to get the start of the second bin
    * Add the bin size to that to get the start of the third bin
    * …
4. Count your data
  - Count how many datapoints in your dataset fit in each bin

[https://www.youtube.com/embed/yxw063NLQ7E?si=Y_nxltRmHOaBNHX2](https://www.youtube.com/embed/yxw063NLQ7E?si=Y_nxltRmHOaBNHX2)

### Step 5: Draw the Histogram

Once your bins are set up and you've counted how many datapoints fall in each one, the last step is to draw the graph:

5. Create a proper scale and labels (just like every other graph we've made)
  - On the x-axis, mark off the boundaries of each bin, in order from smallest to largest
  - On the y-axis, use a scale that reaches at least as high as your largest bin's frequency
6. For each bin, draw a bar reaching up to the frequency (count) for that bin
  - Remember: **the bars must touch**. Don't leave gaps between them.

### A Full Worked Example

Let's put all of these steps together. Suppose we ask 16 students how many minutes it takes them to commute to campus. Here is our data, already sorted from smallest to largest:

$$5, ~7, ~9, ~12, ~14, ~16, ~18, ~20, ~23, ~26, ~29, ~32, ~35, ~38, ~41, ~45$$

**Step 1: Find the range.**

$$Range = Maximum - Minimum = 45 - 5 = 40$$

**Step 2: Determine the number of bins.**

Our sample size is $n = 16$. We need to find out how many times we have to double, starting from 1, to reach 16:

$$1 \rightarrow 2 \rightarrow 4 \rightarrow 8 \rightarrow 16$$

That's 4 doublings, so we will use **4 bins**.

**Step 3: Create the bins.**

$$Bin~Size = \frac{Range}{\text{number of bins}} = \frac{40}{4} = 10$$

Our first bin starts at the minimum value, 5. We keep adding the bin size (10) to get the start of each new bin:

| Bin # | Bin Range |
| ----- | --------- |
| 1     | 5 - 15    |
| 2     | 15 - 25   |
| 3     | 25 - 35   |
| 4     | 35 - 45   |

**Step 4: Count your data.**

Going through our sorted list, we count how many values fall into each bin. (When a value lands exactly on the boundary between two bins, like 35, it belongs to the bin that starts at that number.)

| Bin Range | Values in Bin        | Frequency |
| --------- | --------------------- | --------- |
| 5 - 15    | 5, 7, 9, 12, 14        | 5         |
| 15 - 25   | 16, 18, 20, 23         | 4         |
| 25 - 35   | 26, 29, 32             | 3         |
| 35 - 45   | 35, 38, 41, 45         | 4         |

Notice these frequencies add up to our sample size: $5 + 4 + 3 + 4 = 16$. This is a good way to check your counting.

**Step 5 & 6: Draw the histogram.**

Now we create a proper scale on the x-axis using our bin boundaries (5, 15, 25, 35, 45), a proper scale on the y-axis reaching at least up to 5, and draw a bar for each bin with no gaps between them.

![Histogram of Commute Times](https://drolsonmi.github.io/math1040/Lesson05/images/Fig5_2_CommuteHistogram.png)

That's it! Notice how this histogram already starts to tell a story: most students have a fairly short commute (5-15 minutes), and while there is a smaller group with much longer commutes (35-45 minutes), very few students land right in the middle (25-35 minutes).

### A Note on the Number of Bins

The "doubling" rule we used in Step 2 (formally called **Sturges' Rule**) is a guideline, not an unbreakable law. Its purpose is to keep us from choosing too few bins (which hides the shape of the data by cramming everything into 2 or 3 giant bars) or too many bins (which spreads the data so thin that every bar has a frequency of 0 or 1, and no pattern can be seen). If you find that the suggested number of bins doesn't produce a very readable graph, it is reasonable to adjust the number of bins slightly. Just be consistent, and always list your bin size clearly so your reader knows how the data was grouped.

## Practice

1. The ages of 12 customers at a coffee shop were recorded:

$$22, ~24, ~25, ~29, ~31, ~33, ~35, ~38, ~40, ~44, ~47, ~50$$

Follow the steps above to find the range, the number of bins, and the bin size, and then create a histogram of this data.
  - [After solving on your own, see solution here](https://drolsonmi.github.io/math1040/Lesson05/Solutions/5_2_Solution1.html)

2. A teacher has already grouped her 35 students' exam scores into the frequency table below. Use this table to draw a histogram. (Since the data is already binned for you, you can skip straight to Steps 5 and 6.)

| Exam Score | Frequency |
| ---------- | --------- |
| 50 - 60    | 3         |
| 60 - 70    | 7         |
| 70 - 80    | 12        |
| 80 - 90    | 9         |
| 90 - 100   | 4         |

  - [After solving on your own, see solution here](https://drolsonmi.github.io/math1040/Lesson05/Solutions/5_2_Solution2.html)

## Technology

Just like the graphs in Lesson 4, you can create histograms using Excel, Desmos, or a TI-83/84 calculator.

### Microsoft Excel

Excel has a built-in Histogram chart type:

1. Enter your raw data in a single column
2. Highlight the data
3. Go to **Insert > Chart > Histogram**
4. Excel will automatically choose bins for you, but you can right-click the x-axis and select **Format Axis** to set your own bin width and starting point to match the bins you calculated by hand

### TI-83/84

1. Enter your raw data into a list (e.g., **L1**) using the **STAT > Edit** menu
2. Press **2nd** then **Y=** (STAT PLOT), choose a plot, and turn it **On**
3. Choose the histogram icon as the graph **Type**
4. Set **Xlist** to your data list
5. Press **WINDOW** and set **Xmin** to your minimum value, **Xmax** to a value beyond your maximum, and **Xscl** to your calculated bin size
6. Press **GRAPH** to view the histogram
