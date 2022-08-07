# MechaCar_Statistical_Analysis

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on me and the data analytics team to review the production data for insights that may help the manufacturing team.

# What You're Creating

This new assignment consists of three technical analysis deliverables and a proposal for further statistical study. You’ll submit the following:

## Linear Regression to Predict MPG

![image](https://user-images.githubusercontent.com/103547108/183312339-8041cb56-a53e-440f-b3ea-efc4281ebe95.png)

  Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  - The intercept, vehicle_length, and ground_clearance coeeficients can be said to provide a non-random amount of variance to the mpg values since the non-random   variable is usually 0
  
  Is the slope of the linear model considered to be zero? Why or why not?
  -At a level of 0.05, we are able to reject the 0 hypothesis because of the minimal p-value. The null theory of a linear regression states that the slope (β1) is equal to 0. However, if we reject the null hypothesis, we're stating that alternative (β1 ≠ 0) is true. Proving that the slope is not 0.
  
  Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  - Adjusting R-square to 0.6825 concludes that this linear model predicts the mpg of MechaCar prototypes relatively wel

## Summary Statistics on Suspension Coils

![image](https://user-images.githubusercontent.com/103547108/183312562-65b3ec98-73e3-4590-b752-9e537cb9ab19.png)

![image](https://user-images.githubusercontent.com/103547108/183312566-62685739-ca11-4f79-98f6-78594fc81f2b.png)


The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
 - The variance for the dataset indicates that the current manufacturing data meets the 100 pounds per square inch variance rule. However, when separated into three lots, 'Lot3' demonstrates a much higher variance. Because the lots are chosen randomly, there is a possiblity that a third of the lot does not meet the necessary suspension coils requirement.

## T-Test on Suspension Coils
### T-Test on Entire Lot

![image](https://user-images.githubusercontent.com/103547108/183312683-805a533b-e16e-4be0-89c7-95217d078156.png)

  - From here we can see the true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.
  
  ### T-Test on Three Individual Lots
  
![image](https://user-images.githubusercontent.com/103547108/183312725-0613ead4-7d65-480e-ab54-3e0737bcc9c1.png)

#### Lot 1
  - Lot 1 sample actually has the true sample mean of 1500, again as we saw in the summary statistics above. With a p-Value of 1, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).
  
#### Lot 2
  - Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
 
#### Lot 3
  - However, Lot 3, not surprisingly is a different scenario. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.


Deliverable 4: Design a Study Comparing the MechaCar to the Competition

## Study Design: MechaCar vs Competition
Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

The statistical study design has the following:

A metric to be tested is mentioned
A null hypothesis or an alternative hypothesis is described
A statistical test is described to test the hypothesis
This study would involve collecting data on MechaCar and its comparable models across several different manufacturers over the last 3 years.

What are the competitions' comparable models,
Which cars will MechaCar be competing with head-to-head? which cars will be included in the study?
Which factors will look at the study to determine the relevant to selling price?
Metrics
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

  Safety Feature Rating,
  Current Price (Selling),
  Drive Package,
  Engine (Electric, Hybrid, Gasoline / Conventional),
  Resale Value,
  Average Annual Cost of ownership,
  MPG,
Hypothesis: Null and Alternative
After determining which factors are key for the MechaCar's genre:

Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.

Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.

Statistical Test:
A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price (it may be all of them!)
