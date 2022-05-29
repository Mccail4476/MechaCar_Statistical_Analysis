# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![deliverable_1_linear_regression](https://user-images.githubusercontent.com/99565016/170891890-cd1a7248-3777-4942-ae3a-174f8703cc14.PNG)


***Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?***

It appears that ground clearance & vehicle_length have the lowest probablity of a random event & their respective t-test values are very high, indicating a significant difference.

***Is the slope of the linear model considered to be zero? Why or why not?***

The slope of the linear model should not be zero as there is significance difference. Refer to previous answer.

***Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?***

Given the R-squared value is over 0.7, we can say that there is a strong correlation.


## Summary Statistics on Suspension Coils

![deliverable_2_lots_summary](https://user-images.githubusercontent.com/99565016/170892004-6a2cafbb-548b-498b-8464-46771bbaf89b.PNG)

![deliverable_2_total_summary](https://user-images.githubusercontent.com/99565016/170892007-c76ce81a-a293-4e12-975e-e9088831b759.PNG)


***The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?***

We can see from the total lot data that the variance is ~63 PSI, which falls within the 100 PSI range. This also aplies to Lot 1 & 2, indicating strong precision within those two lots. However, we see that Lot #3 has a variance of ~170 PSI, which goes way over the threshold.


## T-Tests on Suspension Coils

![deliverable_3_lots_ttest](https://user-images.githubusercontent.com/99565016/170892105-a8b92f62-7f24-499e-9197-a1307a538705.PNG)

![deliverable_3_total_ttest](https://user-images.githubusercontent.com/99565016/170892107-1d0f4e70-4afa-4b03-82e1-645edfd678c8.PNG)

***Briefly summarize your interpretation and findings for the t-test results.***

Cut-off for t-test is >2.0.
Cut-off for p-value is >0.5.

For overall lots, we can see that the t-test is ~1.9 with a p-value of ~0.06. No statistical significance.

For Lot 1, t-test is 0 and the p-value is 1. No statistical significance.

For Lot 2, t-test is ~0.5 and the p-value is ~0.6. No statistical significance.

For Lot 3, t-test is ~2.1 and the p-value is 0.04. Since both variables break the cut-off point, there is statistical significance between Lot 3 and the mean. Inspection should start with Lot #3.


## Study Design: MechaCar vs Competition

To design a statistical study that would be used to quantify how the MechaCar would perform against the competitors, there are a few questions to ask.

***What metric or metrics are you going to test?***

An important metric to consider is how much will the car cost in terms of maintenance upkeep? 

***What is the null hypothesis or alternative hypothesis?***

H0: Cost of all MechaCars maintenance upkeep will be the same as the competitors. 

Ha: Cost of all MechaCars maintenance upkeep is high than the competitors because of the quality of parts are not as good, or need specialize mechanics because their internal systems are more sophisticated. The parts could also be harder to find & therefore the mechanics charge more.

***What statistical test would you use to test the hypothesis? And why?***

Since we are comparing MechaCars maintenance upkeep with a different group, hence the competitors' maintenance upkeep, the desired test to use is the two-headed T-test.

***What data is needed to run the statistical test?***

Simply collect how much car owners spend on their maintenance upkeep for MechaCars along with competitors'. Collect large amount of data since people over the world use cars. It would not be wise to use data strictly in a city environment to predict trends for users in the rural area. 
