# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Using the script to calculate the linear regression we get the coefficients as shown:

![Image](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/linear_reg.png)

Using the script to calculate the summary of linear regression model we can determine the p-value and the r-squared value as shown:

![Image](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/summary_LR.png)

* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Vehicle weight, spoiler_angle & AWD provided a non-random amount of variance. The two variables that had the most amount of random variance are ground_clearance and vehicle_length.

* Is the slope of the linear model considered to be zero? Why or why not?

Our slope is not zero just be looking at the p-value, which is less than 0.05.

* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

Our R-squared value is 71%, which means roughly ~71% of the time the model will predict mpg values correctly. There are probably other factors that were not captured in the datasaet that contribute to the mpg variability of the MechaCar prototypes.

## Summary Statistics on Suspension Coils

![total_Summary](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/total_summary.png)

![lot_summary](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/lot_summary.png)

* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Lot 1 and Lot 2 are both within design specifications and have nearly the same exact mean and median. Lot 3 shows the most variance and exceeds the manufacturer's specifications.

## T-Tests on Suspension Coils
Lot 1 and Lot 3 the PSI values are not different from the population mean. However lot 2 the p-value is .347 which means there is evidence that the suspension coil is different from the population mean. All t-tests can be seen below:
### Across all lots:
![mean](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/t_test.png)

### Lot 1
![lot1](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/t_test_lot1.png)

### Lot 2
![lot2](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/t_test_lot2.png)

### Lot 3
![lot3](https://github.com/Vaishali715/MechaCar_Statistical_Analysis/blob/main/Reference%20Images/t_test_lot3.png)

## Study Design: MechaCar vs Competition
* The features that people are interested in, when buying a car are: how much horsepower the car has, the highway fuel efficiency(miles per gallon) and the cost, these are the three factors that go into consumer decision making.

* We can use our tests to see if our MechaCar is much different from the competiton. The null hypothesis is a statement of no difference between a sample mean or proportion and a population mean or proportion. The alternative hypothesis is a contradictory to the null hypothesis. The mean of metricA from the MechaCar can be equal or different than the mean of metricA from the competition. Using the t test we can calculate the p value and depending on this p value we can reject our null hypothesis if p value is smaller than 0.05 and support the alternative hypothesis or accept the null hypothesis and reject the alternative hypothesis. We can make a null hypothesis stating that it is not different from the competition and our alternative would be the opposite.

* As we are comparing the means from two populations we can use two sample t tests. Further, as we want to compare the population means, we can perform a one-tailed t-test.

* To run the statistical test, we will need
    The mean of both samples
    The standard deviation of both samples
    The number of observations