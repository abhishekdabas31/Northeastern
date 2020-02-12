## Hypothesis Testing
A statistical hypothesis test is a method of statistical inference. Commonly, two statistical data sets are compared, or a data set obtained by sampling is compared against a synthetic data set from an idealized model. A hypothesis is proposed for the statistical relationship between the two data sets, and this is compared as an alternative to an idealized null hypothesis that proposes no relationship between two data sets. 

> The null hypothesis is a model of the system under the assumption that the apparent effect is due to chance. For example, if you observed a difference in means, dispersion, or distribution between two groups, the null hypothesis is that the two groups are actually the same.

>>Null Hypothesis (H0): Two variables are independent.
>>Alternate Hypothesis (H1): Two variables are not independent.

# For the purpose of these tests in general
Null: Given two sample means are equal
Alternate: Given two sample means are not equal
## In the theoretical underpinnings, hypothesis tests are based on the notion of critical regions: the null hypothesis is rejected if the test statistic falls in the critical region

## Significance Level
Significance level is the threshold at which we cap our risk of falsely rejecting a null hypothesis.

`After carrying out a test, if the probability of getting a result as strange as the one you observe is lower than the significance level, you reject the null hypothesis in favor of the alternative. If the probability is higher than  𝛼 , then the null hypothesis is in effect and the result is not strange at all.`

## Critical Value - 
A critical value is a point (or points) on the scale of the test statistic beyond which we reject the null hypothesis, and, is derived from the level of significance α of the test. Critical value can tell us, what is the probability of two sample means belonging to the same distribution. Higher, the critical value means lower the probability of two samples belonging to same distribution. The general critical value for a two-tailed test is 1.96, which is based on the fact that 95% of the area of a normal distribution is within 1.96 standard deviations of the mean.

## Confidence intervals
In statistics, a confidence interval (CI) is a type of interval estimate of a population parameter. It provides an interval estimate for lower or upper confidence bounds. For $\beta_1$, usually referred to as a confidence interval and is typically +/-0.5% (a 99% confidence interval),+/-1% (a 98% confidence interval),+/-2.5% (a 95% confidence interval) or +/-5% (a 90% confidence interval). The lower and upper confidence bounds need not be equal, and they can be any number such that the confidence interval not exceed 100%

## P-Value
p-value which is the specific probability of getting results as extreme as we have if the null hypothesis were true.
It is the total probability of achieving a value so rare and even rarer.
`The critical value can be any value between 0 and 1. It is typically chosen as 0.05.`
we can say that we have a confidence interval of 95%. If you decrease your critical value to 0.01, you make your Hypothesis Test more strict as you now want the new p-value to be even lower (less than 0.01) if you want to reject your null hypothesis. This means that your confidence interval will be 99%.

Z= X-μ / σ
X = Sample mean, μ=Population mean, σ=Standard deviation
This P-Value is calculated using the Z score we just found. Each Z-score has a corresponding P-Value. This can be found using any statistical software like R or even from the Z-Table.

Now if this P-Value comes to be less than critical value — signifying that probability of achieving this desired solution was so unlikely that it was indeed not by luck, we can reject our null hypothesis. Now, we cannot say that we accept our alternate hypothesis as statistics is a game of inferences and we can never be 100% sure. But, as we set had set our confidence interval, we can be 95% or even 99% sure. This is where errors creep in!

# Chi-Square Test
A Chi-Square test is a test of statistical significance for categorical variables.

# Z-test
In a z-test, the sample is assumed to be normally distributed. A z-score is calculated with population parameters such as “population mean” and “population standard deviation” and is used to validate a hypothesis that the sample drawn belongs to the same population.
Null: Sample mean is same as the population mean
Alternate: Sample mean is not same as the population mean

# T-test
A t-test is used to compare the mean of two given samples. Like a z-test, a t-test also assumes a normal distribution of the sample. A t-test is used when the population parameters (mean and standard deviation) are not known.

# ANOVA
ANOVA, also known as analysis of variance, is used to compare multiple (three or more) samples with a single test. There are 2 major flavors of ANOVA
1. One-way ANOVA: It is used to compare the difference between the three or more samples/groups of a single independent variable.
2. MANOVA: MANOVA allows us to test the effect of one or more independent variable on two or more dependent variables. In addition, MANOVA can also detect the difference in co-relation between dependent variables given the groups of independent variables.
The hypothesis being tested in ANOVA is
Null: All pairs of samples are same i.e. all sample means are equal
Alternate: At least one pair of samples is significantly different

# Chi-Square Test
Chi-square test is used to compare categorical variables. There are two type of chi-square test
1. Goodness of fit test, which determines if a sample matches the population.
2. A chi-square fit test for two independent variables is used to compare two variables in a contingency table to check if the data fits.
a. A small chi-square value means that data fits
b. A high chi-square value means that data doesn’t fit.
The hypothesis being tested for chi-square is
Null: Variable A and Variable B are independent
Alternate: Variable A and Variable B are not independent.

# Note: As one can see from the above examples, in all the tests a statistic is being compared with a critical value to accept or reject a hypothesis. However, the statistic and way to calculate it differ depending on the type of variable, the number of samples being analyzed and if the population parameters are known. Thus depending upon such factors a suitable test and null hypothesis is chosen.


## Type 1 and Type 2 Errors
Now as I said, we can never be 100% sure. There is always a possibility that your conclusion is wrong and the ground truth, the reality, is totally opposite.
If your significance level is 0.05, that means that you indeed have a 5% chance to be wrong! Meaning, you rejected your null hypothesis when it was actually true in reality. This is a Type 1 Error. Hence, the probability of committing a Type 1 error is α.
Conversely, you could also conclude that your null hypothesis is true or in statistical words, you fail to reject your null hypothesis when in reality it was actually false. This is a case of Type 2 Error. The probability of committing a Type 2 error is explained by Beta — β.





Credit :- 
1. https://towardsdatascience.com/the-only-theorem-data-scientists-need-to-know-a50a263d013c
2. https://towardsdatascience.com/everything-you-need-to-know-about-hypothesis-testing-part-i-4de9abebbc8a
3. https://towardsdatascience.com/hypothesis-testing-the-what-why-and-how-867d382b99ca
4. https://towardsdatascience.com/statistical-tests-when-to-use-which-704557554740