# Choosing the Right Plot for Automobile Data

**Getting to Know Your Data**

**Objective:** Create and interpret different plots, choose suitable visualizations for different attribute types, and explore automobile characteristics and prices.

## Dataset

Load the automobile dataset. You can find this dataset here: 
https://github.com/m-mahdavi/teaching/tree/main/datasets

The dataset contains these columns:

```text
index,company,body-style,wheel-base,length,engine-type,num-of-cylinders,horsepower,average-mileage,price
```

## Scenario

You work as a data analyst for a car dealership. The manager wants to understand the available vehicles, compare prices across vehicle categories, and investigate how vehicle characteristics relate to price. Prepare plots that answer these questions.

## Task 1: Understand the Attributes

Inspect the dataset and classify each attribute before creating charts.

**Instructions:**

1. Identify which attributes are nominal, ordinal, or numeric. Identify discrete and continuous attributes.
2. Explain whether numerical operations are meaningful for every column containing numbers.
3. Check for missing values, duplicate records, and numbers stored as text.

**Questions:**

- Which attributes describe categories, and which describe quantities?
- Does every categorical attribute have a meaningful order?


## Task 2: Bar Chart: Which Body Styles Are Most Common?

**Create:** A bar chart showing the number of vehicles in each body-style category.

**Instructions:**

1. Count the records in each body-style category.
2. Check for inconsistent category labels before counting.
3. Arrange the bars in an order that supports comparison.
4. Label the axes and provide an informative title.

**Questions:**

- Which body style appears most frequently?
- Are the categories evenly represented?
- Why is a bar chart appropriate for this attribute?
- Why would a histogram be inappropriate for body style?
- Can the most frequent body style in this dataset be described as the best-selling body style? Explain.

## Task 3: Histogram: How Are Vehicle Prices Distributed?

**Create:** Two price histograms, using approximately **5 bins** and **15 bins**.

**Instructions:**

1. Use the same valid price observations in both histograms.
2. Keep the displayed price range consistent.
3. Compare the distribution shapes revealed by the two binning choices.
4. Calculate the mean and median price to support your interpretation.

**Questions:**

- Is the price distribution approximately symmetric or skewed?
- Do you see possible peaks, gaps, or extreme values?
- Which binning choice communicates the distribution more clearly?
- How does the relationship between the mean and median support your interpretation?
- Why would a separate bar for every distinct price be less useful?

## Task 4: Scatter Plot: How Does Horsepower Relate to Price?

**Create:** A scatter plot with **horsepower on the horizontal axis** and **price on the vertical axis**.

**Instructions:**

1. Plot one point per vehicle with valid values for both attributes.
2. Use smaller markers or transparency if points overlap.
3. Use a different color for each body style
4. Identify any observations that appear unusual relative to the overall pattern.

**Questions:**

- Is the relationship upward, downward, curved, or unclear?
- Are there clusters or isolated observations?
- Does body style help explain any visible grouping?
- Can you conclude that increasing horsepower causes a particular increase in price? Explain.

## Submission

Provide the plots and your answers to the accompanying questions. Use readable titles, labeled axes, units where verified, and legends where necessary. Support your conclusions with the displayed data.

