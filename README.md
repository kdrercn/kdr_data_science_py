# Data Science

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

 -----------------------------------------------------------

  ## Chapter 2 : Data and Sampling Distributions

  -----------------------------------------------------------

  ### Random Sampling and Sample Bias

  **Sample**:
  A subset from a larger data set.

  **Population**:
  The larger data set or idea of a data set.

  **N (n)**:
  The size of the population (sample).

  **Random Sampling**:
  Drawing elements into a sample at random.

  **Stratified Sampling**:
  Dividing the population into strata and randomly sampling from each strata.

  **Simple Random Sample**:
  The sample that results from random sampling without stratifying the population.

  **Sample Bias**:
  A sample that misrepresents the population.

  :star: **KEY IDEAS** :
  * Even in the era of big data, random sampling remains an important arrow in the data scientist’s quiver.
  * Bias occurs when measurements or observations are systematically in error because they are not representative of the full population.
  * Data quality is often more important than data quantity, and random sampling can reduce bias and facilitate quality improvement that would be prohibitively expensive.

  -----------------------------------------------------------

  ### Selection Bias

  **Bias**:
  Systematic error.

  **Data snooping**:
  Extensive hunting through data in search of something interesting.

  **Vast Search Effect**:
  Bias or nonreproducibility resulting from repeated data modeling, or modeling data with large numbers of predictor variables.

  **Reagression to the Mean**:
  Regression to the mean refers to a phenomenon involving successive measurements on a given variable: extreme observations tend to be followed by more central ones. Attaching special focus and meaning to the extreme value can lead to a form of selection bias.

  :star: **KEY IDEAS** :
  * Specifying a hypothesis, then collecting data following randomization and random sampling principles, ensures against bias.
  * All other forms of data analysis run the risk of bias resulting from the data collection/analysis process (repeated running of models in data mining, data snooping in research, and after-the-fact selection of interesting events).

  -----------------------------------------------------------

  ### Sampling Distribution of a Statistic

  **Sample Statistic**:
  A metric calculated for a sample of data drawn from a larger population.

  **Data Distribution**:
  The frequency distribution of individual values in a data set.

  **Sampling Distribution**:
  The frequency distribution of a sample statistic over many samples or resamples.

  **Central Limit Theorem**:
  The tendency of the sampling distribution to take on a normal shape as sample size rises.

  **Standard Error**:
  The variability (standard deviation) of a sample statistic over many samples (not to be confused with standard deviation, which, by itself, refers to variability of individual data values).

  ![Standard error formula.](/im/stderr.png)
  
  :star2: **STANDARD DEVIATION VERSUS STANDARD ERROR**
  Do not confuse standard deviation (which measures the variability of individual data points) with standard error (which measures the variability of a sample metric).

  :star: **KEY IDEAS** :
  * The frequency distribution of a sample statistic tells us how that metric would turn out differently from sample to sample.
  * This sampling distribution can be estimated via the bootstrap, or via formulas that rely on the central limit theorem.
  * A key metric that sums up the variability of a sample statistic is its standard error.

  -----------------------------------------------------------

  ### The Bootstrap

  **Bootstrap Sample**:
  A sample taken with replacement from an observed data set.

  **Resampling**:
  The process of taking repeated samples from observed data; includes both bootstrap and permutation (shuffling) procedures.

  ![Bootstrap - Theory](/im/bootstrap.png)
  
  :star2: The bootstrap does not compensate for a small sample size; it does not create new data, nor does it fill in holes in an existing data set. It merely informs us about how lots of additional samples would behave when drawn from a population like our original sample.

  :star: **KEY IDEAS** :
  * The bootstrap (sampling with replacement from a data set) is a powerful tool for assessing the variability of a sample statistic.
  * The bootstrap can be applied in similar fashion in a wide variety of circumstances, without extensive study of mathematical approximations to sampling distributions.
  * It also allows us to estimate sampling distributions for statistics where no mathematical approximation has been developed.
  * When applied to predictive models, aggregating multiple bootstrap sample predictions (bagging) outperforms the use of a single model.

  -----------------------------------------------------------

  ### Confidence Intervals

  Frequency tables, histograms, boxplots, and standard errors are all ways to understand the potential error in a sample estimate. Confidence intervals are another.

  **Confidence Level**
  The percentage of confidence intervals, constructed in the same way from the same population, expected to contain the statistic of interest.

  **Interval Endpoints**:
  The top and bottom of the confidence interval.

  :star2: What we are really interested in when we have a sample result is “what is the probability that the true value lies within a certain interval?” This is not really the question that a confidence interval answers, but it ends up being how most people interpret the answer.

  :star2: For a data scientist, a confidence interval is a tool to get an idea of how variable a sample result might be. Data scientists would use this information not to publish a scholarly paper or submit a result to a regulatory agency (as a researcher might), but most likely to communicate the potential error in an estimate, and, perhaps, learn whether a larger sample is needed.


  :star: **KEY IDEAS** :
  * Confidence intervals are the typical way to present estimates as an interval range.
  * The more data you have, the less variable a sample estimate will be.
  * The lower the level of confidence you can tolerate, the narrower the confidence interval will be.
  * The bootstrap is an effective way to construct confidence intervals..

  -----------------------------------------------------------

  ### Normal Distribution

  **Error**:
  The difference between a data point and a predicted or average value.

  **Standardize**:
  Subtract the mean and divide by the standard deviation.

  **z-score**:
  The result of standardizing an individual data point.

  **Standard Normal**:
  A normal distribution with mean = 0 and standard deviation = 1.

  **QQ-Plot**:
  A plot to visualize how close a sample distribution is to a normal distribution.

  :star2: Converting data to z-scores (i.e., standardizing or normalizing the data) does not make the data normally distributed. It just puts the data on the same scale as the standard normal distribution, often for comparison purposes.

  :star: **KEY IDEAS** :
  * The normal distribution was essential to the historical development of statistics, as it permitted mathematical approximation of uncertainty and variability.
  * While raw data is typically not normally distributed, errors often are, as are averages and totals in large samples.
  * To convert data to z-scores, you subtract the mean of the data and divide by the standard deviation; you can then compare the data to a normal distribution.

  -----------------------------------------------------------

  ### Long-Tailed Distributions

  **Tail**:
  The long narrow portion of a frequency distribution, where relatively extreme values occur at low frequency.

  **Skew**:
  Where one tail of a distribution is longer than the other.

  :star: **KEY IDEAS** :
  * Most data is not normally distributed.
  * Assuming a normal distribution can lead to underestimation of extreme events (“black swans”).

  -----------------------------------------------------------

  ### Student’s t-Distribution

  The t-distribution is a normally shaped distribution, but a bit thicker and longer on the tails. It is used extensively in depicting distributions of sample statistics. Distributions of sample means are typically shaped like a t-distribution, and there is a family of t-distributions that differ depending on how large the sample is. The larger the sample, the more normally shaped the t-distribution becomes.

  **Degrees of Freedom**:
  A parameter that allows the t-distribution to adjust to different sample sizes, statistics, and number of groups.

  :star2: What do data scientists need to know about the t-distribution and the central limit theorem? Not a whole lot. These distributions are used in classical statistical inference, but are not as central to the purposes of data science. Understanding and quantifying uncertainty and variation are important to data scientists, but empirical bootstrap sampling can answer most questions about sampling error. However, data scientists will routinely encounter t-statistics in output from statistical software and statistical procedures in R, for example in A-B tests and regressions, so familiarity with its purpose is helpful

  :star: **KEY IDEAS** :
  * The t-distribution is actually a family of distributions resembling the normal distribution, but with thicker tails.
  * It is widely used as a reference basis for the distribution of sample means, differerences between two sample means, regression parameters, and more.

  -----------------------------------------------------------

  ### Binomial Distribution

  **Trial**:
  An event with a discrete outcome (e.g., a coin flip).

  **Success**:
  The outcome of interest for a trial.

  **Binomial**:
  Having two outcomes.

  **Binomial Trial**:
  A trial with two outcomes (Bernoulli trial).

  **Binomial Distribution**:
  Distribution of number of successes in x trials (Bernoulli distribution).

  :star2: Calculating binomial probabilities with large sample sizes is computationally demanding, and most statistical procedures use the normal distribution, with mean and variance, as an approximation.

  :star: **KEY IDEAS** :
  * Binomial outcomes are important to model, since they represent, among other things, fundamental decisions (buy or don’t buy, click or don’t click, survive or die, etc.).
  * A binomial trial is an experiment with two possible outcomes: one with probability p and the other with probability 1 – p.
  * With large n, and provided p is not too close to 0 or 1, the binomial distribution can be approximated by the normal distribution.

  -----------------------------------------------------------

  ### Poisson and Related Distributions

  **Lambda**:
  The rate (per unit of time or space) at which events occur.

  **Poisson Distribution**:
  The frequency distribution of the number of events in sampled units of time or space.

  **Exponential distribution**:
  The frequency distribution of the time or distance from one event to the next event.

  :star2: A key assumption in any simulation study for either the Poisson or exponential distribution is that the rate, λ, remains constant over the period being considered. This is rarely reasonable in a global sense; for example, traffic on roads or data networks varies by time of day and day of week. However, the time periods, or areas of space, can usually be divided into segments that are sufficiently homogeneous so that analysis or simulation within those periods is valid.

  **Weibull distribution**:
  A generalized version of the exponential, in which the event rate is allowed to shift over time.

  :star2: The Weibull distribution is an extension of the exponential distribution, in which the event rate is allowed to change, as specified by a shape parameter, β. If β > 1, the probability of an event increases over time, if β < 1, it decreases. 

  :star: **KEY IDEAS** :
  * For events that occur at a constant rate, the number of events per unit of time or space can be modeled as a Poisson distribution.
  * In this scenario, you can also model the time or distance between one event and the next as an exponential distribution.
  * A changing event rate over time (e.g., an increasing probability of device failure) can be modeled with the Weibull distribution.

  -----------------------------------------------------------
  
  **Example**:
  [ex2.1.r](/ex2.1.r).

  -----------------------------------------------------------
  
  ### SUMMARY
  **In the era of big data, the principles of random sampling remain important when accurate estimates are needed. Random selection of data can reduce bias and yield a higher quality data set than would result from just using the conveniently available data. Knowledge of various sampling and data generating distributions allows us to quantify potential errors in an estimate that might be due to random variation. At the same time, the bootstrap (sampling with replacement from an observed data set) is an attractive “one size fits all” method to determine possible error in sample estimates.**

  -----------------------------------------------------------

 