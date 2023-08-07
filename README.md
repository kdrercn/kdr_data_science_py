# Data Science

# First run [0.r](/0.r). to install packages etc. and change the paths.

-----------------------------------------------------------

## Statistics
### From Book : Practical Statistics for Data Scientists

-----------------------------------------------------------

## Chapter 1 : Exploratory Data Analysis

### Estimates of Location
**Mean** : 
The sum of all values divided by the number of values. Average.

![Mean formula.](/im/mean.png)

**Weighted mean** : 
The sum of all values times a weight divided by the sum of the weights.

![Weighted Mean formula.](/im/weightedmean.png)

**Median** : 
The value such that one-half of the data lies above and below.

**Weighted Median** : 
The value such that one-half of the sum of the weights lies above and below.

**Trimmed mean** : 
The average of all values after dropping a fixed number of extreme values

![Trimmed Mean formula.](/im/trimmedmean.png)
 
**Robust** :
 Not sensitive to extreme values.
 
**Outlier** :
 A data value that is very different from most of the data.
 
 **Example**:
 [ex1.1.r](/ex1.1.r).
 
 -----------------------------------------------------------
### Estimates of Variability

**Deviations**:
The difference between the observed values and the estimate of location.

**Variance**:
The sum of squared deviations from the mean divided by n – 1 where n is the number of data values. Mean-squared-error.

![Variance formula.](/im/var.png)

**Standard Deviation**:
The square root of the variance.

![Standard Deviation formula.](/im/std.png)

:star: The standard deviation is much easier to interpret than the variance since it is on the same scale as the original data.

**Mean Absolute Deviation**:
The mean of the absolute value of the deviations from the mean.

![Mean Absolute Deviation formula.](/im/meanabsdev.png)

**Median absolute deviation from the median**:
The median of the absolute value of the deviations from the median.

**Range**:
The difference between the largest and the smallest value in a data set.

**Order Statistics**:
Metrics based on the data values sorted from smallest to biggest.

**Percentile**:
The value such that P percent of the values take on this value or less and (100–P) percent take on this value or more.

**Interquartile Range**:
The difference between the 75th percentile and the 25th percentile. IQR.

 **Example**:
 [ex1.2.r](/ex1.2.r).
 
 -----------------------------------------------------------
 
 ### Exploring the Data Distribution
 
 **Boxplot**:
 A plot to visualize the distribution of data.
 
 **Frequency Table**:
 A tally of the count of numeric data values that fall into a set of intervals (bins).
 
 **Histogram**:
 A plot of the frequency table with the bins on the x-axis and the count (or proportion) on the y-axis.
 
 **Density Plot**:
 A smoothed version of the histogram, often based on a kernal density estimate.
 
 **Example**:
  [ex1.3.r](/ex1.3.r).
  
 :star: **KEY IDEAS** :
* A frequency histogram plots frequency counts on the y-axis and variable values on the x-axis; it gives a sense of the distribution of the data at a glance.
* A frequency table is a tabular version of the frequency counts found in a histogram.
* A boxplot — with the top and bottom of the box at the 75th and 25th percentiles, respectively —also gives a quick sense of the distribution of the data; it is often used in side-by-side displays to compare distributions.
* A density plot is a smoothed version of a histogram; it requires a function to estimate a plot based on the data (multiple estimates are possible, of course)

 -----------------------------------------------------------
 
 ### Exploring Binary and Categorical Data
 
 **Mode**:
 The most commonly occurring category or value in a data set.
 
 **Expected Value:
 When the categories can be associated with a numeric value, this gives an average value based on a category’s probability of occurrence.
 
 **Bar charts**:
 The frequency or proportion for each category plotted as bars.
 
 **Pie charts**:
 The frequency or proportion for each category plotted as wedges in a pie.
 
 **Example**:
 [ex1.4.r](/ex1.4.r).

 :star: **KEY IDEAS** :
* Categorical data is typically summed up in proportions, and can be visualized in a bar chart.
* Categories might represent distinct things (apples and oranges, male and female), levels of a factor variable (low, medium, and high), or numeric data that has been binned.
* Expected value is the sum of values times their probability of occurrence, often used to sum up factor variable levels.
 
 -----------------------------------------------------------
 
 ### Correlation
 
 **Correlation coefficient**:
 A metric that measures the extent to which numeric variables are associated with one another (ranges from –1 to +1).
 
 :star: The correlation coefficient always lies between +1 (perfect positive correlation) and –1 (perfect negative correlation); 0 indicates no correlation.
 
 ![Correlation formula.](/im/corr.png)
 
 **Correlation matrix**:
 A table where the variables are shown on both rows and columns, and the cell values are the correlations between the variables.
 
 **Scatterplot**:
 A plot in which the x-axis is the value of one variable, and the y-axis the value of another.
 
 **Example**:
 [ex1.5.r](/ex1.5.r).
 
  :star: **KEY IDEAS** :
* The correlation coefficient measures the extent to which two variables are associated with one another.
* When high values of v1 go with high values of v2, v1 and v2 are positively associated.
* When high values of v1 are associated with low values of v2, v1 and v2 are negatively associated.
* The correlation coefficient is a standardized metric so that it always ranges from –1 (perfect negative correlation) to +1 (perfect positive correlation).
* A correlation coefficient of 0 indicates no correlation, but be aware that random arrangements of data will produce both positive and negative values for the correlation coefficient just by chance.
 
 -----------------------------------------------------------
 
 ### Exploring Two or More Variables
 
 **Contingency Tables**:
 A tally of counts between two or more categorical variables.
 
 **Hexagonal Binning**:
 A plot of two numeric variables with the records binned into hexagons.
 
 **Contour plots**:
 A plot showing the density of two numeric variables like a topographical map.
 
 **Violin plots**:
 Similar to a boxplot but showing the density estimate.
 
   :star: **KEY IDEAS** :
* Hexagonal binning and contour plots are useful tools that permit graphical examination of two numeric variables at a time, without being overwhelmed by huge amounts of data.
* Contingency tables are the standard tool for looking at the counts of two categorical variables.
* Boxplots and violin plots allow you to plot a numeric variable against a categorical variable.

 -----------------------------------------------------------
 
 ### SUMMARY
 **The key idea of EDA is that the first and most important step in any project based on data is to look at the data. By summarizing and visualizing the data, you can gain valuable intuition and understanding of the project.**
 