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
## Chapter 4 : Regression and Prediction

-----------------------------------------------------------

Perhaps the most common goal in statistics is to answer the question: Is the variable X associated with a variable Y, and, if so, what is the relationship and can we use it to predict Y?

### Simple Linear Regression

Simple linear regression models the relationship between the magnitude of one variable and that of a second — for example, as X increases, Y also increases. Or as X increases, Y decreases. Correlation is another way to measure how two variables are related: see the section “Correlation”. The difference is that while correlation measures the strength of an association between two variables, regression quantifies the nature of the relationship

**Response**:
The variable we are trying to predict.

**Independent variable**:
The variable used to predict the response.

**Record**:predicted values
The vector of predictor and outcome values for a specific individual or case.

**Intercept**:
The intercept of the regression line — that is, the predicted value when x=0.

**Regression Coefficient**:
The slope of the regression line.

**Fitted values**
The estimates Y'i obtained from the regression line (Predicted value).

**Residuals**:
The difference between the observed values and the fitted values.

**Least Squares**:
The method of fitting a regression by minimizing the sum of squared residuals.

### The Regression Equation

Simple linear regression estimates exactly how much Y will change when X changes by a certain amount. With the correlation coefficient, the variables X and Y are interchangable. With regression, we are trying to predict the Y variable from X using a linear relationship.

![Regression Equation formula.](/im/regeq.png)
 
### Fitted Values and Residuals
 
In general, the data doesn’t fall exactly on a line, so the regression equation should include an explicit error term : e¡.

![Explicit Error formula.](/im/experr.png)

The fitted values, also referred to as the predicted values, are typically denoted by (Y-hat). These are given by:

![Fitted Values formula.](/im/fitted.png)

:star2: **HAT NOTATION: ESTIMATES VERSUS KNOWN VALUES**: The “hat” notation is used to differentiate between estimates and known values.

We compute the residuals ê¡ by subtracting the predicted values from the original data:

![Residuals formula.](/im/residual.png)
 
### Least Squares

![Residual Sum of Squares formula.](/im/rss.png)

The estimates ![b hat 0](/im/b0.png) and ![b hat 1](/im/b1.png) are the values that minimize RSS.

![Coefficients' formula.](/im/b1b0.png)

:star2: With the advent of big data, computational speed is still an important factor. Least squares, like the mean, are sensitive to outliers, although this tends to be a signicant problem only in small or moderate-sized problems

-----------------------------------------------------------

:star: **KEY IDEAS** :
* The regression equation models the relationship between a response variable Y and a predictor ariable X as a line.
* A regression model yields fitted values and residuals — predictions of the response and the errors of the predictions.
* Regression models are typically fit by the method of least squares.
* Regression is used both for prediction and explanation.

-----------------------------------------------------------

### Multiple Linear Regression

When there are multiple predictors, the equation is simply extended to accommodate them:

![Multiple Linear Regression formula.](/im/mls.png)

Instead of a line, we now have a linear model — the relationship between each coefficient and its variable (feature) is linear.

**Root Mean Squared Error**:
The square root of the average squared error of the regression (this is the most widely used metric to compare regression models).

**Residual Standard Error**:
The same as the root mean squared error, but adjusted for degrees of freedom.

**R-squared**:
The proportion of variance explained by the model, from 0 to 1.

**t-statistic**:
The coefficient for a predictor, divided by the standard error of the coefficient, giving a metric to compare the importance of variables in the model.

**Weighted Regression**:
Regression with the records having different weights.

All of the other concepts in simple linear regression, such as fitting by least squares and the definition of fitted values and residuals, extend to the multiple linear regression setting. For example, the fitted values are given by:

![Multiple Linear Regression Fitted Values formula.](/im/mlsfv.png)

### Assessing the Model

The most important performance metric from a data science perspective is root mean squared error, or RMSE. RMSE is the square root of the average squared error in the predicted ![y hat i.](/im/yi.png) values:

![RMSE formula.](/im/rmse.png)

This measures the overall accuracy of the model.

Similar to RMSE is the residual standard error, or RSE. In this case we have p predictors, and the RSE is given by:

![RSE formula.](/im/rse.png)

The only difference is that the denominator is the degrees of freedom, as opposed to number of records.

:star2: In practice, for linear regression, the difference between RMSE and RSE is very small, particularly for big data applications.

R-squared ranges from 0 to 1 and measures the proportion of variation in the data that is accounted for in the model. It is useful mainly in explanatory uses of regression where you want to assess how well the model fits the data. The formula for R-squared is:

![r-squared formula.](/im/r2.png)

t-statistic:

![t-statistic formula.](/im/tstat.png)

The t-statistic — and its mirror image, the p-value — measures the extent to which a coefficient is “statistically significant” — that is, outside the range of what a random chance arrangement of predictor and target variable might produce.

:star2: **The higher the t-statistic (and the lower the p-value), the more significant the predictor.**

:warning: Data scientists primarily focus on the t-statistic as a useful guide for whether to include a predictor in a model or not. High t-statistics (which go with p-values near 0) indicate a predictor should be retained in a model, while very low t-statistics indicate a predictor could be dropped. 

### Cross-Validation

Cross-validation extends the idea of a holdout sample to multiple sequential holdout samples. The algorithm for basic k-fold cross-validation is as follows:

1. Set aside 1/k of the data as a holdout sample.

2. Train the model on the remaining data.

3. Apply (score) the model to the 1/k holdout, and record needed model assessment metrics.

4. Restore the first 1/k of the data, and set aside the next 1/k (excluding any records that got picked the first time). 

5. Repeat steps 2 and 3.

6. Repeat until each record has been used in the holdout portion.

7. Average or otherwise combine the model assessment metrics.

### Model Selection and Stepwise Regression

Adding more variables, however, does not necessarily mean we have a better model. Statisticians use the principle of Occam’s razor to guide the choice of a model: all things being equal, a simpler model should be used in preference to a more complicated model.

A metric called AIC (Akaike’s Information Criteria) that penalizes adding terms to a model. In the case of regression, AIC has the form:

![AIC formula.](/im/aic.png)

Where p is the number of variables and n is the number of records. The goal is to find the model that minimizes AIC; models with k more extra variables are penalized by 2k.

:star: **AIC, BIC AND MALLOWS CP**:
The formula for AIC may seem a bit mysterious, but in fact it is based on asymptotic results in information theory. There are several variants to AIC:

* AICc: a version of AIC corrected for small sample sizes.
* BIC or Bayesian information criteria: similar to AIC with a stronger penalty for including additional variables to the model.
* Mallows Cp: A variant of AIC developed by Colin Mallows.

Data scientists generally do not need to worry about the differences among these in-sample metrics or the underlying theory behind them.

**How do we find the model that minimizes AIC?**

One approach is to search through all possible models, called all subset regression. This is computationally expensive and is not feasible for problems with large data and many variables. An attractive alternative is to use stepwise regression, which successively adds and drops predictors to find a model that lowers AIC.

In forward selection, you start with no predictors and add them one-by-one, at each step adding the predictor that has the largest contribution to , stopping when the contribution is no longer statistically significant. In backward selection, or backward elimination, you start with the full model and take away predictors that are not statistically significant until you are left with a model in which all predictors are statistically significant.

:warning: Stepwise regression and all subset regression are in-sample methods to assess and tune models. This means the model selection is possibly subject to overfitting and may not perform as well when applied to new data. One common approach to avoid this is to use cross-validation to validate the models. 

### Weighted Regression

Data scientists may find weighted regression useful in two cases:

* Inverse-variance weighting when different observations have been measured with different precision.

* Analysis of data in an aggregated form such that the weight variable encodes how many original observations each row in the aggregated data represents.

For example, with the housing data, older sales are less reliable than more recent sales.

-----------------------------------------------------------

:star: **KEY IDEAS** :
* Multiple linear regression models the relationship between a response variable Y and multiple predictor variables.
* The most important metrics to evaluate a model are root mean squared error (RMSE) and R-squared .
* The standard error of the coefficients can be used to measure the reliability of a variable’s contribution to a model.
* Stepwise regression is a way to automatically determine which variables should be included in the model.
* Weighted regression is used to give certain records more or less weight in fitting the equation.

-----------------------------------------------------------

### Prediction Using Regression

**Prediction Interval**:
An uncertainty interval around an individual predicted value

**Extrapolation**:
Extension of a model beyond the range of the data used to fit it.

### The Dangers of Extrapolation

As an extreme case, suppose model_lm ([ex4.3.r](/ex4.3.r) is used to predict the value of a 5,000-square-foot empty lot. In such a case, all the predictors related to the building would have a value of 0 and the regression equation would yield an absurd prediction of – 521,900 + 5,000 × –.0605 = –$522,202. Why did this happen? The data contains only parcels with buildings — there are no records corresponding to vacant land. Consequently, the model has no information to tell it how to predict the sales price for vacant land.

### Confidence and Prediction Intervals

Much of statistics involves understanding and measuring variability (uncertainty). The t-statistics and p-values reported in regression output deal with this in a formal way, which is sometimes useful for variable selection. More useful metrics are confidence intervals, which are uncertainty intervals placed around regression coefficients and predictions. An easy way to understand this is via the bootstrap.

Here is a bootstrap algorithm for generating confidence intervals for regression parameters (coefficients) for a data set with P predictors and n records (rows):
1. Consider each row (including outcome variable) as a single “ticket” and place all the n tickets in a box.
2. Draw a ticket at random, record the values, and replace it in the box.
3. Repeat step 2 n times; you now have one bootstrap resample.
4. Fit a regression to the bootstrap sample, and record the estimated coefficients.
5. Repeat steps 2 through 4, say, 1,000 times.
6. You now have 1,000 bootstrap values for each coefficient; find the appropriate percentiles for each one (e.g., 5th and 95th for a 90% confidence interval).

The individual data point error can be thought of as follows: even if we knew for certain what the regression equation was (e.g., if we had a huge number of records to fit it), the actual outcome values for a given set of predictor values will vary. For example, several houses — each with 8 rooms, a 6,500 square foot lot, 3 bathrooms, and a basement — might have different values. We can model this individual error with the residuals from the fitted values. The bootstrap algorithm for modeling both the regression model error and the individual data point error would look as follows

1. Take a bootstrap sample from the data (spelled out in greater detail earlier).
2. Fit the regression, and predict the new value.
3. Take a single residual at random from the original regression fit, add it to the predicted value, and record the result.
4. Repeat steps 1 through 3, say, 1,000 times.
5. Find the 2.5th and the 97.5th percentiles of the results.

:star2:  **PREDICTION INTERVAL OR CONFIDENCE INTERVAL?**: Prediction interval pertains to uncertainty around a single value, while a confidence interval pertains to a mean or other statistic calculated from multiple values. Thus, a prediction interval will typically be much wider than a confidence interval for the same value. 

-----------------------------------------------------------

:star: **KEY IDEAS** :
* Extrapolation beyond the range of the data can lead to error.
* Confidence intervals quantify uncertainty around regression coefficients.
* Prediction intervals quantify uncertainty in individual predictions.
* Most software, R included, will produce prediction and confidence intervals in default or specified output, using formulas.
* The bootstrap can also be used; the interpretation and idea are the same.

-----------------------------------------------------------

### Factor Variables in Regression

Factor variables, also termed categorical variables, take on a limited number of discrete values.
For example, a loan purpose can be “debt consolidation,” “wedding,” “car,” and so on. 
The binary (yes/no) variable, also called an indicator variable, is a special case of a factor variable. 
Regression requires numerical inputs, so factor variables need to be recoded to use in the model. The most common approach is to convert a variable into a set of binary dummy variables.

**Dummy Variables**:
Binary 0–1 variables derived by recoding factor data for use in regression and other models

**Reference Coding**:
The most common type of coding used by statisticians, in which one level of a factor is used as a reference and other factors are compared to that level

**One Hot Encoder**:
A common type of coding used in the machine learning community in which all factors levels are retained. While useful for certain machine learning algorithms, this approach is not appropriate for multiple linear regression.

**Deviation Coding**:
A type of coding that compares each level against the overall mean as opposed to the reference level.

### Dummy Variables Representation

The output from the R regression shows two coefficients corresponding to PropertyType: PropertyTypeSingle Family and PropertyTypeTownhouse. There is no coefficient of Multiplex since it is implicitly defined when PropertyTypeSingle Family == 0 and PropertyTypeTownhouse == 0. The coefficients are interpreted as relative to Multiplex, so a home that is Single Family is worth almost $85,000 less, and a home that is Townhouse is worth over $150,000 less.

:star2: With the exception of ordered factors, data scientists will generally not encounter any type of coding besides reference coding or one hot encoder.

### Factor Variables with Many Levels

### Ordered Factor Variables

Some factor variables reflect levels of a factor; these are termed ordered factor variables or ordered categorical variables. For example, the loan grade could be A, B, C, and so on — each grade carries more risk than the prior grade. 

-----------------------------------------------------------

:star: **KEY IDEAS** :
* Factor variables need to be converted into numeric variables for use in a regression.
* The most common method to encode a factor variable with P distinct values is to represent them using P-1 dummy variables.
* A factor variable with many levels, even in very big data sets, may need to be consolidated into a variable with fewer levels.
* Some factors have levels that are ordered and can be represented as a single numeric variable.

-----------------------------------------------------------

### Interpreting the Regression Equation

In data science, the most important use of regression is to predict some dependent (outcome) variable. In some cases, however, gaining insight from the equation itself to understand the nature of the relationship between the predictors and the outcome can be of value.

**Correlated Variables**:
When the predictor variables are highly correlated, it is difficult to interpret the individual coefficients.

**Multicollinearity**:
When the predictor variables have perfect, or near-perfect, correlation, the regression can be unstable or impossible to compute.

**Confounding Variables**:
An important predictor that, when omitted, leads to spurious relationships in a regression equation.

**Main Effects**:
The relationship between a predictor and the outcome variable, independent from other variables.

**Interactions**:
An interdependent relationship between two or more predictors and the response.

### Correlated Predictors

The coefficient for Bedrooms is negative! This implies that adding a bedroom to a house will reduce its value. How can this be? This is because the predictor variables are correlated: larger houses tend to have more bedrooms, and it is the size that drives house value, not the number of bedrooms. Consider two homes of the exact same size: it is reasonable to expect that a home with more, but smaller, bedrooms would be considered less desirable.

### Multicollinearity

An extreme case of correlated variables produces multicollinearity — a condition in which there is redundance among the predictor variables. Perfectmulticollinearity occurs when one predictor variable can be expressed as a linear combination of others. 

Multicollinearity occurs when:
* A variable is included multiple times by error.
* P dummies, instead of P – 1 dummies, are created from a factor variable
* Two variables are nearly perfectly correlated with one another.

### Confounding Variables

ZipGroup is clearly an important variable: a home in the most expensive zip code group is estimated to have a higher sales price by almost $340,000. The coefficients of SqFtLot and Bathrooms are now positive and adding a bathroom increases the sale price by $7,500.

### Interactions and Main Effects

For example, the model fit to the King County Housing Data in “Confounding Variables” includes several variables as main effects, including ZipCode. Location in real estate is everything, and it is natural to presume that the relationship between, say, house size and the sale price depends on location. A big house built in a low-rent district is not going to retain the same value as a big house built in an expensive area. You include interactions between variables in R using the \* operator. For the King County data, the following fits an interaction between SqFtTotLiving and ZipGroup.

Location and house size appear to have a strong interaction. For a home in the lowest ZipGroup, the slope is the same as the slope for the main effect SqFtTotLiving, which is $177 per square foot. For a home in the highest ZipGroup, the slope is the sum of the main effect plus SqFtTotLiving:ZipGroup5, or $177 + $230 = $447 per square foot. In other words, adding a square foot in the most expensive zip code group boosts the predicted sale price by a factor of almost 2.7, compared to the boost in the least expensive zip code group.

-----------------------------------------------------------

:star: **KEY IDEAS** :
* Because of correlation between predictors, care must be taken in the interpretation of the coefficients in multiple linear regression.
* Multicollinearity can cause numerical instability in fitting the regression equation.
* A confounding variable is an important predictor that is omitted from a model and can lead to a regression equation with spurious relationships.
* An interaction term between two variables is needed if the relationship between the variables and the response is interdependent.

-----------------------------------------------------------

### Testing the Assumptions: Regression Diagnostics

These steps do not directly address predictive accuracy, but they can provide useful insight in a predictive setting.
 
**Standardized Residuals**:
Residuals divided by the standard error of the residuals

**Outliers**:
Records (or outcome values) that are distant from the rest of the data (or the predicted outcome).

**Influential Value**:
A value or record whose presence or absence makes a big difference in the regression equation.

**Leverage**:
The degree of influence that a single record has on a regression equation.

**Non-normal Residuals**:
Non-normally distributed residuals can invalidate some technical requirements of regression, but are usually not a concern in data science.

**Heteroskedasticity**:
When some ranges of the outcome experience residuals with higher variance (may indicate a predictor missing from the equation).

**Partial Residual Plots**:
A diagnostic plot to illuminate the relationship between the outcome variable and a single predictor.

### Outliers

Generally speaking, an extreme value, also called an outlier, is one that is distant from most of the other observations. 
You can detect outliers by examining the standardized residual, which is the residual divided by the standard error of the residuals.

The biggest overestimate from the model is more than four standard errors above the regression line, corresponding to an overestimate of $757,753. 

In this case, it appears that there is something wrong with the record: a house of that size typically sells for much more than $119,748 in that zip code.

Below image shows an excerpt from the statuatory deed from this sale: it is clear that the sale involved only partial interest in the property. In this case, the outlier corresonds to a sale that is anomalous and should not be included in the regression.

![Outlier.](/im/outlier.png) 

:star: For big data problems, outliers are generally not a problem in fitting the regression to be used in predicting new data. However, outliers are central to anomaly detection, where finding outliers is the whole point. The outlier could also correspond to a case of fraud or an accidental action. In any case, detecting outliers can be a critical business need.

### Influential Values

A value whose absence would significantly change the regression equation is termed an infuential observation.

The solid line corresponds to the regression with all the data, while the dashed line corresonds to the regression with the point in the upper-right removed. Clearly, that data value has a huge influence on the regression even though it is not associated with a large outlier (from the full regression). This data value is considered to have high leverage on the regression.

![Influential removed.](/im/inftable.png) 

Above table compares the regression with the full data set and with highly influential data points removed. The regression coefficient for Bathrooms changes quite dramatically.

### Heteroskedasticity, Non-Normality and Correlated Errors

Heteroskedasticity is the lack of constant residual variance across the range of the predicted values. In other words, errors are greater for some portions of the range than for others.

Evidently, the variance of the residuals tends to increase for higher-valued homes, but is also large for lower-valued homes. This plot indicates that lm_98105 has heteroskedastic errors.

:star2: **WHY WOULD A DATA SCIENTIST CARE ABOUT HETEROSKEDASTICITY?**
Heteroskedasticity indicates that prediction errors differ for different ranges of the predicted value, and may suggest an incomplete model. For example, the heteroskedasticity in lm_98105 may indicate that the regression has left something unaccounted for in high- and low-range homes.

:star: Even though a regression may violate one of the distributional assumptions, should we care? Most often in data science, the interest is primarily in predictive accuracy, so some review of heteroskedasticity may be in order. You may discover that there is some signal in the data that your model has not captured. Satisfying distributional assumptions simply for the sake of validating formal statistical inference (p-values, F-statistics, etc.), however, is not that important for the data scientist

:star2: **SCATTERPLOT SMOOTHERS**
Regression is about modeling the relationship between the response and predictor variables. In evaluating a regression model, it is useful to use a scatterplot smoother to visually highlight relationships between two variables

### Partial Residual Plots and Nonlinearity

Partial residual plots are a way to visualize how well the estimated fit explains the relationship between a predictor and the outcome.

Along with detection of outliers, this is probably the most important diagnostic for data scientists. 

The basic idea of a partial residual plot is to isolate the relationship between a predictor variable and the response, taking into account all of the other predictor variables.

![Partial Residual Formula](/im/partres.png) 

The partial residual is an estimate of the contribution that SqFtTotLiving adds to the sales price. The relationship between SqFtTotLiving and the sales price is evidently nonlinear. The regression line underestimates the sales price for homes less than 1,000 square feet and overestimates the price for homes between 2,000 and 3,000 square feet.

There are too few data points above 4,000 square feet to draw conclusions for those homes.

:star2: This nonlinearity makes sense in this case: adding 500 feet in a small home makes a much bigger difference than adding 500 feet in a large home. This suggests that, instead of a simple linear term for SqFtTotLiving, a nonlinear term should be considered

-----------------------------------------------------------

:star: **KEY IDEAS** :
* While outliers can cause problems for small data sets, the primary interest with outliers is to identify problems with the data, or locate anomalies.
* Single records (including regression outliers) can have a big influence on a regression equation with small data, but this effect washes out in big data.
* If the regression model is used for formal inference (p-values and the like), then certain assumptions about the distribution of the residuals should be checked. In general, however, the distribution of residuals is not critical in data science.
* The partial residuals plot can be used to qualitatively assess the fit for each regression term, possibly leading to alternative model specification.

-----------------------------------------------------------

### Polynomial and Spline Regression

The relationship between the response and a predictor variable is not necessarily linear. The response to the dose of a drug is often nonlinear: doubling the dosage generally doesn’t lead to a doubled response. The demand for a product is not a linear function of marketing dollars spent since, at some point, demand is likely to be saturated. There are several ways that regression can be extended to capture these nonlinear effects

**Polynomial Regression**:
Adds polynomial terms (squares, cubes, etc.) to a regression.

**Spline Regression**:
Fitting a smooth curve with a series of polynomial segments.

**Knots**:
Values that separate spline segments

**Generalized Additive Models**:
Spline models with automated selection of knots.

:star2: Nonlinear regression models are harder and computationally more intensive to fit, since they require numerical optimization. For this reason, it is generally preferred to use a linear model if possible

### Polynomial

Polynomial regression involves including polynomial terms to a regression equation.

![Polynomial Regression Formula](/im/polyreg.png) 

The fitted line more closely matches the smooth of the partial residuals as compared to a linear fit.

### Splines

Polynomial regression only captures a certain amount of curvature in a nonlinear relationship. Adding in higher-order terms, such as a cubic quartic polynomial, often leads to undesirable “wiggliness” in the regression equation. An alternative, and often superior, approach to modeling nonlinear relationships is to use splines.

Splines provide a way to smoothly interpolate between fixed points. Splines were originally used by draftsmen to draw a smooth curve, particularly in ship and aircraft building.

The technical definition of a spline is a series of piecewise continuous polynomials.

The polynomial pieces are smoothly connected at a series of fixed points in a predictor variable, referred to as knots. Formulation of splines is much more complicated than polynomial regression. 

:star2: Two parameters need to be specified: the degree of the polynomial and the location of the knots. In this case, the predictor SqFtTotLiving is included in the model using a cubic spline (degree=3). By default, bs places knots at the boundaries; in addition, knots were also placed at the lower quartile, the median quartile, and the upper quartile.

In contrast to the polynomial model, the spline model more closely matches the smooth, demonstrating the greater flexibility of splines. In this case, the line more closely fits the data. 

Does this mean the spline regression is a better model? Not necessarily: it doesn’t make economic sense that very small homes (less than 1,000 square feet) would have higher value than slightly larger homes. This is possibly an artifact of a confounding variable;

### Generalized Additive Models (GAM)

Suppose you suspect a nonlinear relationship between the response and a predictor variable, either by a priori knowledge or by examining the regression diagnostics. Polynomial terms may not flexible enough to capture the relationship, and spline terms require specifying the knots. Generalized additive models, or GAM, are a technique to automatically fit a spline regression. 

-----------------------------------------------------------

:star: **KEY IDEAS** :
* Outliers in a regression are records with a large residual.
* Multicollinearity can cause numerical instability in fitting the regression equation
* A confounding variable is an important predictor that is omitted from a model and can lead to a regression equation with spurious relationships.
* An interaction term between two variables is needed if the effect of one variable depends on the level of the other.
* Polynomial regression can fit nonlinear relationships between predictors and the outcome variable.
* Splines are series of polynomial segments strung together, joining at knots
* Generalized additive models (GAM) automate the process of specifying the knots in splines.

-----------------------------------------------------------
 
### SUMMARY
**The fundamental form is linear: each predictor variable has a coefficient that describes a linear relationship between the predictor and the outcome.**
**More advanced forms of regression, such as polynomial and spline regression, permit the relationship to be nonlinear.**

-----------------------------------------------------------