# MechaCar_Statistical_Analysis

Click here to view my Challenge RScript: [RScript](https://github.com/jzaragoza21/MechaCar_Statistical_Analysis/blob/main/MechaCar_Challenge.R)

## Project Overview

The objective of this project is to perform an analysis on metrics that impact the manufacturing of the new MechaCar prototype and compare with vehicle performnace across other manufacturing lots. Specifically, we will employ mulitple linear regression, summary statistics and t-tests to analyze vehicle length, vehicle weight, spoiler angle, ground clearance, AWD and MPG. 

## Linear Regression to Predict MPG

![Linear_Regression_MPG](https://github.com/jzaragoza21/MechaCar_Statistical_Analysis/blob/main/Resources/Linear_Regression_MPG.PNG)

The three takeaways addressing the three questions are as follows:

  - Typically, the variance of a non-random variable is most of the time O, and provided this, the coefficients of the intercept, vehicle length and ground clearance can be said to give a non-random amount of variance to the MPG values.
  - In measuring by a significance level of .05, we are able to reject the null hypothesis given the super tiny p-value of 0.0000000000535. The null hypothesis of a linear regression states that the slope (β1) is equal to 0. That said, if we reject the null hypthesis, we're stating that alternative (β1 ≠ 0) is true. Consequently proving the slope is not 0.
  -  According to this regression model, the multiple R-squared of .71 shows there's a strong correlation but multiple R-aquared increases as more variables are passed through the regression. Having said that, adjusted R-squared controls against this increase, and adds penalties for the number of predictors in the model and therefore making it a better predictor. The adjusted R-square of 0.6825 demonstrates this linear model predicts the MPG of the MechaCar quite well.


## Summary Statistics on Suspension Coils

![total_summary](https://github.com/jzaragoza21/MechaCar_Statistical_Analysis/blob/main/Resources/total_summary.PNG)
![lot_summary](https://github.com/jzaragoza21/MechaCar_Statistical_Analysis/blob/main/Resources/lot_summary.PNG)

The summary statistics analysis above shows that manfacturing data for the suspension coils does not in fact exceed the variance of 100 pounds per square inch. Having said that, when the lots are broken down into 3 lots, the third lot stands out as exceeding the variance of 100 pounds per square inch quite significantly. As a result, one could suspect that a third of the lots could exceed the suspension coils variance limitation.

## T-Test on Suspension Coils

### T-Test on Entire Lot

![t-test_EntireLot](https://github.com/jzaragoza21/MechaCar_Statistical_Analysis/blob/main/Resources/t-test.PNG)

Given the measurement of success by a significance level of .05, we fail to reject the null hypothesis with a p-value of .06. As a result, we can't reject the fact that the sample mean is perhaps the equaivalent to the population mean. A notable feature however is the confidence interval is slender, which usually implies a greater accuracy overall.

### T-Test on the Three Smaller Lotes

![t-test_3lots](https://github.com/jzaragoza21/MechaCar_Statistical_Analysis/blob/main/Resources/Lots_t-test.PNG)

#### Lot 1

Measuring by a significance level of 0.05, we fail to reject the null hypothesis given the p-value equals 1. However, there is interesting correlation between the p-value and the confidence interval in that as the p-value increases, the confidence interval decreases - which can indicate there's more accuracy in precicting the true population mean

#### Lot 2

Measuring by a significance level of 0.05, we fail to reject the null hypothesis given the p-value equals .61. Again, the confidence interval is quite narrow with Lot 2 as well.

#### Lot 3

Measuring by a significance level of 0.05, we can reject the null hypothesis given the p-value equals .04. Additionally, the mean of the Lot 3 sample is also significantly smaller in comparison to the previous two lots. Especially important is that Lot 3 does not include the predicted population mean unlike the first two.

## Study Design: MechaCar vs Competition

In addition to the prior analysis, we can perform more analysis to compare MechaCar against its competitors. Specifically, we can run linear regression on city and highway fuel efficiency given the cost of gas right now. This, coupled with safety and cost, are the primary reasons why people purchase cars in today's market. 

  - City and highway fuel efficiency are the dependent variables
  - Selling Price: independent variable
  - Horse power: independent variable
  - AWD capabilities: independent variable
  - MPG: Independent variable
