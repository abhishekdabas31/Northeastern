## Hypothesis Testing
A statistical hypothesis test is a method of statistical inference. Commonly, two statistical data sets are compared, or a data set obtained by sampling is compared against a synthetic data set from an idealized model. A hypothesis is proposed for the statistical relationship between the two data sets, and this is compared as an alternative to an idealized null hypothesis that proposes no relationship between two data sets. 

## Significance Level
Significance level is the threshold at which we cap our risk of falsely rejecting a null hypothesis.

`After carrying out a test, if the probability of getting a result as strange as the one you observe is lower than the significance level, you reject the null hypothesis in favor of the alternative. If the probability is higher than  𝛼 , then the null hypothesis is in effect and the result is not strange at all.`

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

## Type 1 and Type 2 Errors
Now as I said, we can never be 100% sure. There is always a possibility that your conclusion is wrong and the ground truth, the reality, is totally opposite.
If your significance level is 0.05, that means that you indeed have a 5% chance to be wrong! Meaning, you rejected your null hypothesis when it was actually true in reality. This is a Type 1 Error. Hence, the probability of committing a Type 1 error is α.
Conversely, you could also conclude that your null hypothesis is true or in statistical words, you fail to reject your null hypothesis when in reality it was actually false. This is a case of Type 2 Error. The probability of committing a Type 2 error is explained by Beta — β.





Credit :- 
1. https://towardsdatascience.com/the-only-theorem-data-scientists-need-to-know-a50a263d013c
2. https://towardsdatascience.com/everything-you-need-to-know-about-hypothesis-testing-part-i-4de9abebbc8a
3. https://towardsdatascience.com/hypothesis-testing-the-what-why-and-how-867d382b99ca