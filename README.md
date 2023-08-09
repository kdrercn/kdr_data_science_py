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
 
 **Expected Value**:
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
  
  :star2: **STANDARD DEVIATION VERSUS STANDARD ERROR**:
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
  
  ### SUMMARY
  **In the era of big data, the principles of random sampling remain important when accurate estimates are needed. Random selection of data can reduce bias and yield a higher quality data set than would result from just using the conveniently available data. Knowledge of various sampling and data generating distributions allows us to quantify potential errors in an estimate that might be due to random variation. At the same time, the bootstrap (sampling with replacement from an observed data set) is an attractive “one size fits all” method to determine possible error in sample estimates.**

  -----------------------------------------------------------

 
## Chapter 3 : Statistical Experiments and Significance Testing

-----------------------------------------------------------

  This process starts with a hypothesis (“drug A is better than the existing standard drug,” “price A is more profitable than the existing price B”). An experiment (it might be an A/B test) is designed to test the hypothesis — designed in such a way that, hopefully, will deliver conclusive results. The data is collected and analyzed, and then a conclusion is drawn. 

  ![The classical statistical inference pipeline](/im/pipeline.png)

  ### A/B Testing

  An A/B test is an experiment with two groups to establish which of two treatments, products, procedures, or the like is superior. 

  **Treatment**:
  Something (drug, price, web headline) to which a subject is exposed.

  **Treatment Group**:
  A group of subjects exposed to a specific treatment.

  **Control Group**:
  A group of subjects exposed to no (or standard) treatment.

  **Randomization**:
  The process of randomly assigning subjects to treatments.

  **Subjects**:
  The items (web visitors, patients, etc.) that are exposed to treatments.

  **Test Statistic**:
  The metric used to measure the effect of the treatment.

  :star: **Some examples of A/B testing include** :
  + Testing two soil treatments to determine which produces better seed germination
  + Testing two therapies to determine which suppresses cancer more effectively
  + Testing two prices to determine which yields more net profit
  + Testing two web headlines to determine which produces more clicks
  + Testing two web ads to determine which generates more conversions

  :star2: **Why Have a Control Group?**:
  Why not skip the control group and just run an experiment applying the treatment of interest to only one group, and compare the outcome to prior experience? Without a control group, there is no assurance that “other things are equal” and that any difference is really due to the treatment (or to chance). When you have a control group, it is subject to the same conditions (except for the treatment of interest) as the treatment group. If you simply make a comparison to “baseline” or prior experience, other factors, besides the treatment, might differ

  :star2: Data scientists are less interested in the question:
  Is the difference between price A and price B statistically significant?
  than in the question:
  Which, out of multiple possible prices, is best?

  :star: **KEY IDEAS** :
  * Subjects are assigned to two (or more) groups that are treated exactly alike, except that the treatment under study differs from one to another.
  * Ideally, subjects are assigned randomly to the groups.

  -----------------------------------------------------------

  ### Hypothesis Tests (significance tests)

  Purpose is to help you learn whether random chance might be responsible for an observed effect.

  **Null Hypothesis**:
  The hypothesis that chance is to blame.

  **Alternative Hypothesis**:
  Counterpoint to the null (what you hope to prove).

  **One-way Test**:
  Hypothesis test that counts chance results only in one direction.

  **Two-way test**:
  Hypothesis test that counts chance results in two directions.

  :star2: **MISINTERPRETING RANDOMNESS**: You can observe the human tendency to underestimate randomness in this experiment. Ask several friends to invent a series of 50 coin flips: have them write down a series of random Hs and Ts. Then ask them to actually flip a coin 50 times and write down the results. Have them put the real coin flip results in one pile, and the made-up results in another. It is easy to tell which results are real: the real ones will have longer runs of Hs or Ts. In a set of 50 real coin flips, it is not at all unusual to see five or six Hs or Ts in a row. However, when most of us are inventing random coin flips and we have gotten three or four Hs in a row, we tell ourselves that, for the series to look random, we had better switch to T. The other side of this coin, so to speak, is that when we do see the real-world equivalent of six Hs in a row (e.g., when one headline outperforms another by 10%), we are inclined to attribute it to something real, not just chance.

  :star2: Statistical hypothesis testing was invented as a way to protect researchers from being fooled by random chance.

  :star: **KEY IDEAS** :
  * A null hypothesis is a logical construct embodying the notion that nothing special has happened, and any effect you observe is due to random chance.
  * The hypothesis test assumes that the null hypothesis is true, creates a “null model” (a probability model), and tests whether the effect you observe is a reasonable outcome of that model.

  -----------------------------------------------------------

  ### Resampling

  There are two main types of resampling procedures: the bootstrap and permutation tests. The bootstrap is used to assess the reliability of an estimate; it was discussed in the previous chapter ([see](#The Bootstrap)). Permutation tests are used to test hypotheses, typically involving two or more groups, and we discuss those in this section.

  **Permutation test**:
  The procedure of combining two or more samples together, and randomly (or exhaustively) reallocating the observations to resamples.

  **With or without replacement**:
  In sampling, whether or not an item is returned to the sample before the next draw.


  -----------------------------------------------------------

  ### Permutation Test

  1. Combine the results from the different groups in a single data set.
  2. Shuffle the combined data, then randomly draw (without replacing) a resample of the same size as group A.
  3. From the remaining data, randomly draw (without replacing) a resample of the same size as group B.
  4. Do the same for groups C, D, and so on. 
  5. Whatever statistic or estimate was calculated for the original samples (e.g., difference in group proportions), calculate it now for the resamples, and record; this constitutes one permutation iteration.
  6. Repeat the previous steps R times to yield a permutation distribution of the test statistic.

  :star2: Now go back to the observed difference between groups and compare it to the set of permuted differences. If the observed difference lies well within the set of permuted differences, then we have not proven anything — the observed difference is within the range of what chance might produce. However, if the observed difference lies outside most of the permutation distribution, then we conclude that chance is not responsible. In technical terms, the difference is statistically significant.

  -----------------------------------------------------------

  ### Exhaustive and Bootstrap Permutation Test

  In addition to the preceding random shuffling procedure, also called a random permutation test or a randomization test, there are two variants of the permutation test:
  * An exhaustive permutation test :

  In an exhaustive permutation test, instead of just randomly shuffling and dividing the data, we actually figure out all the possible ways it could be divided. This is practical only for relatively small sample sizes. 

  * A bootstrap permutation test :

  In a bootstrap permutation test, the draws outlined in steps 2 and 3 of the random permutation test are made with replacement instead of without replacement. In this way the resampling procedure models not just the random element in the assignment of treatment to subject, but also the random element in the selection of subjects from a population.

  :star: **KEY IDEAS** :
  * In a permutation test, multiple samples are combined, then shuffled.
  * The shuffled values are then divided into resamples, and the statistic of interest is calculated.
  * This process is then repeated, and the resampled statistic is tabulated.
  * Comparing the observed value of the statistic to the resampled distribution allows you to judge whether an observed difference between samples might occur by chance.

  -----------------------------------------------------------

  ### Statistical Significance and P-Values

  Statistical significance is how statisticians measure whether an experiment (or even a study of existing data) yields a result more extreme than what chance might produce. If the result is beyond the realm of chance variation, it is said to be statistically significant.

  **P-value**:
  Short for "probability value," is a measure used in statistical hypothesis testing to assess the strength of evidence against a null hypothesis. P-value helps you determine whether the results you've observed are statistically significant or if they could have occurred due to random chance.

  **Alpha**:
  The probability threshold of “unusualness” that chance results must surpass, for actual outcomes to be deemed statistically significant.

  **Type 1 Error**:
  Mistakenly concluding an effect is real (when it is due to chance).

  **Type 2 Error**:
  Mistakenly concluding an effect is due to chance (when it is real).
  
  :star: **KEY IDEAS** :
  * Significance tests are used to determine whether an observed effect is within the range of chance variation for a null hypothesis model.
  * The p-value is the probability that results as extreme as the observed results might occur, given a null hypothesis model.
  * The alpha value is the threshold of “unusualness” in a null hypothesis chance model.
  * Significance testing has been much more relevant for formal reporting of research than for data science (but has been fading recently, even for the former).

  -----------------------------------------------------------

  ### t-Tests

  **Test Statistic**:
  A metric for the difference or effect of interest.

  **t-statistic**:
  A standardized version of the test statistic.

  **t-distribution**:
  A reference distribution (in this case derived from the null hypothesis), to which the observed t-statistic can be compared.
  
  :star: **KEY IDEAS** :
  * Before the advent of computers, resampling tests were not practical and statisticians used standard reference distributions.
  * A test statistic could then be standardized and compared to the reference distribution.
  * One such widely used standardized statistic is the t-statistic.

  -----------------------------------------------------------

  ### Multiple Testing

  **Type 1 error**:
  Mistakenly concluding that an effect is statistically significant.

  **False Discovery Rate**:
  Across multiple tests, the rate of making a Type 1 error.

  **Adjustment of p-values**:
  Accounting for doing multiple tests on the same data.

  **Overfitting**:
  Fitting the noise.

  :star: **KEY IDEAS** :
  * Multiplicity in a research study or data mining project (multiple comparisons, many variables, many models, etc.) increases the risk of concluding that something is significant just by chance.
  * For situations involving multiple statistical comparisons (i.e., multiple tests of significance) there are statistical adjustment procedures.
  * In a data mining situation, use of a holdout sample with labeled outcome variables can help avoid misleading results.

  -----------------------------------------------------------
  
  ### Degrees of Freedom

  :star: **KEY IDEAS** :
  * The number of degrees of freedom (d.f.) forms part of the calculation to standardize test statistics so they can be compared to reference distributions (t-distribution, F-distribution, etc.).
  * The concept of degrees of freedom lies behind the factoring of categorical variables into n – 1 indicator or dummy variables when doing a regression (to avoid multicollinearity)

  -----------------------------------------------------------
  
  ### ANOVA

  Suppose that, instead of an A/B test, we had a comparison of multiple groups, say A-B-C-D, each with numeric data. The statistical procedure that tests for a statistically significant difference among the groups is called analysis of variance, or ANOVA.

  **Pairwise Comparison**:
  A hypothesis test (e.g., of means) between two groups among multiple groups.

  **Omnibus Test**:
  A single hypothesis test of the overall variance among multiple group means.

  **Decomposition of Variance**:
  Separation of components. contributing to an individual value (e.g., from the overall average, from a treatment mean, and from a residual error).

  **F-statistic**:
  A standardized statistic that measures the extent to which differences among group means exceeds what might be expected in a chance model.

  **SS**:
  “Sum of squares,” referring to deviations from some average value.
  
  ### F-Statistic
  
  Just like the t-test can be used instead of a permutation test for comparing the mean of two groups, there is a statistical test for ANOVA based on the F-statistic.
  
  F-statistic is based on the ratio of the variance across group means (i.e., the treatment effect) to the variance due to residual error. The higher this ratio, the more statistically significant the result. 
  
  ### Two-Way ANOVA
  
  The A-B-C-D test just described is a “one-way” ANOVA, in which we have one factor (group) that is varying. We could have a second factor involved — say, “weekend versus weekday” — with data collected on each combination (group A weekend, group A weekday, group B weekend, etc.). This would be a “two-way ANOVA,” and we would handle it in similar fashion to the one-way ANOVA by identifying the “interaction effect.” After identifying the grand average effect, and the treatment effect, we then separate the weekend and the weekday observations for each group, and find the difference between the averages for those subsets and the treatment average.
  
  You can see that ANOVA, then two-way ANOVA, are the first steps on the road toward a full statistical model, such as regression and logistic regression, in which multiple factors and their effects can be modeled.
  
    :star: **KEY IDEAS** :
  * ANOVA is a statistical procedure for analyzing the results of an experiment with multiple groups.
  * It is the extension of similar procedures for the A/B test, used to assess whether the overall variation among groups is within the range of chance variation.
  * A useful outcome of an ANOVA is the identification of variance components associated with group treatments, interaction effects, and errors.

  ### Chi-Square Test

  The chi-square test is used with count data to test how well it fits some expected distribution. The most common use of the chi-square statistic in statistical practice is with "rxc" contingency tables, to assess whether the null hypothesis of independence among variables is reasonable.

  **Chi-square Statistic**:
  A measure of the extent to which some observed data departs from expectation.

  **Expectation or expected**:
  How we would expect the data to turn out under some assumption, typically the null hypothesis.

  **d.f.**:
  Degrees of freedom.

  :star2: "r x c" means “rows by columns” — a 2×3 table has two rows and three columns.

  ### Chi-Square Test: A Resampling Approach

  The Pearson residual is defined as:

  ![Pearson Residual formula.](/im/pearsonresidual.png)

  The chi-squared statistic is defined as the sum of the squared Pearson residuals:

  ![Chi-squared Statistic formula.](/im/chisq.png)
  
  ###  Chi-Squared Test: Statistical Theory
  
  Asymptotic statistical theory shows that the distribution of the chi-squared statistic can be approximated by a chi-square distribution. The appropriate standard chi- square distribution is determined by the degrees of freedom.
  
  d.f. = (r - 1) X (c - 1)
  
  ### Fisher’s Exact Test

  The chi-square distribution is a good approximation of the shuffled resampling test just described, except when counts are extremely low (single digits, especially five or fewer). In such cases, the resampling procedure will yield more accurate p-values.

  -----------------------------------------------------------
  
  ### Relevance for Data Science

  :star2: Most standard uses of the chi-square test, or Fisher’s exact test, are not terribly relevant for data science. In most experiments, whether A-B or A-B-C…, the goal is not simply to establish statistical significance, but rather to arive at the best treatment. For this purpose, multi-armed bandits (see “Multi-Arm Bandit Algorithm”) offer a more complete solution.

  :star2: Chi-square tests are used widely in research by investigators in search of the elusive statistically significant p-value that will allow publication. Chi-square tests, or similar resampling simulations, are used in data science applications more as a filter to determine whether an effect or feature is worthy of further consideration than as a formal test of significance.

    :star: **KEY IDEAS** :
  * A common procedure in statistics is to test whether observed data counts are consistent with an assumption of independence (e.g., propensity to buy a particular item is independent of gender).
  * The chi-square distribution is the reference distribution (which embodies the assumption of independence) to which the observed calculated chi-square statistic must be compared.

  -----------------------------------------------------------
  
  ### Multi-Arm Bandit Algorithm

  Multi-arm bandits offer an approach to testing, especially web testing, that allows explicit optimization and more rapid decision making than the traditional statistical approach to designing experiments.

  **Multi-arm Bandit**:
  An imaginary slot machine with multiple arms for the customer to choose from, each with different payoffs, here taken to be an analogy for a multitreatment experiment.

  **Arm**:
  A treatment in an experiment (e.g., “headline A in a web test”).

  **Win**:
  The experimental analog of a win at the slot machine (e.g., “customer clicks on the link”).

  You can probably perceive several difficulties with that approach. First, our answer may be inconclusive: “effect not proven.” In other words, the results from the experiment may suggest an effect, but if there is an effect, we don’t have a big enough sample to prove it (to the satisfaction of the traditional statistical standards). What decision do we take? Second, we might want to begin taking advantage of results that come in prior to the conclusion of the experiment. Third, we might want the right to change our minds or to try something different based on additional data that comes in after the experiment is over.data science (and business in general) not so worried about statistical significance, but more concerned with optimizing overall effort and results.

  Here is one simple algorithm, the epsilon-greedy algorithm for an A/B test:
  1. Generate a random number between 0 and 1

  2. f the number lies between 0 and epsilon (where epsilon is a number between 0 and 1, typically fairly small), flip a fair coin (50/50 probability), and:

  a. If the coin is heads, show offer A.
  b. If the coin is tails, show offer B.

  3. If the number is ≥ epsilon, show whichever offer has had the highest response rate to date.

  Bandit algorithms can efficiently handle 3+ treatments and move toward optimal selection of the “best.” For traditional statistical testing procedures, the complexity of decision making for 3+ treatments far outstrips that of the traditional A/B test, and the advantage of bandit algorithms is much greater.

    :star: **KEY IDEAS** :
  * Traditional A/B tests envision a random sampling process, which can lead to excessive exposure to the inferior treatment.
  * Multi-arm bandits, in contrast, alter the sampling process to incorporate information learned during the experiment and reduce the frequency of the inferior treatment.
  * They also facilitate efficient treatment of more than two treatments.
  * There are different algorithms for shifting sampling probability away from the inferior treatment(s) and to the (presumed) superior one.

  -----------------------------------------------------------
  
  ### Power and Sample Size

  **Effect Size**:
  The minimum size of the effect that you hope to be able to detect in a statistical test, such as “a 20% improvement in click rates”.

  **Power**:
  The probability of detecting a given effect size with a given sample size.

  **Significance Level**:
  The statistical significance level at which the test will be conducted.

  ### Sample Size

  The most common use of power calculations is to estimate how big a sample you will need.

  In summary, for calculating power or required sample size, there are four moving parts:

  * Sample size
  * Effect size you want to detect
  * Significance level (alpha) at which the test will be conducted
  * Power

  Specify any three of them, and the fourth can be calculated. 
  
  :star: **KEY IDEAS** :
  * Finding out how big a sample size you need requires thinking ahead to the statistical test you plan to conduct.
  * You must specify the minimum size of the effect that you want to detect.
  * You must also specify the required probability of detecting that effect size (power).
  * Finally, you must specify the significance level (alpha) at which the test will be conducted.

  -----------------------------------------------------------
  
  ### SUMMARY
  
  The principles of experimental design — randomization of subjects into two or more groups receiving different treatments — allow us to draw valid conclusions about how well the treatments work. It is best to include a control treatment of “making no change.” The subject of formal statistical inference — hypothesis testing, p-values, t-tests, and much more along these lines — occupies much time and space in a traditional statistics course or text, and the formality is mostly unneeded from a data science perspective. However, it remains important to recognize the role that random variation can play in fooling the human brain. Intuitive resampling procedures (permutation and bootstrap) allow data scientists to gauge the extent to which chance variation can play a role in their data analysis.
  
    -----------------------------------------------------------
