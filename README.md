# MechaCar_Statistical_Analysis

## Overview of the Analysis:
Using Linear Regression to Predict MPG, Summary Statistics on Suspension Coils, T-Test on Suspension Coils, at the end we need to study MechaCar vs competion

### Purpose:

1.Perform linear regression to get variables in the dataset predicting the mpg of MechaCar prototypes,
2. Collect statistics on the pounds per square inch (PSI) of the suspension coils from the lots,
3. Using t-tests to get if the manufacturing lots are statistically different from the mean of the population,
4. Statistical study as a comparison MechaCar vehicles vs vehicle from other manufacturers.



## Results:

## Linear Regression to Predict MPG

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879902-e84fdeab-99b6-4ccd-a7d6-a37a966e7354.png"> 
</p>

- Variables/coefficients providing a nonrandom amount of variance to the mpg values in the dataset? 

The most significant variables are the Vehicle Length and the Ground Clearance. A linear regression model run on these variables vs figures for MPG resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. 
Intercept was statistically significant, showing hidden factors not shown in in the dataset, anyway demonstrate a big impact on.

The slope of the linear model is not be zero, while  p-value of 5.35x10-11, is lower than even an extreme level of significance, null hypothesis is rejected. This means that the relationship between our variables and consume per gallon is subject to more than random chance.

- Does this linear model predict the mpg of MechaCar prototypes effectively? Why or why not? 

Thought with untouched factors, this model predicts the mpg of the MechaCar prototype with some effectiveness. The r-squared value of 0.7149, model is 71% accurate.

<br>

## Summary Statistics on Suspension Coils

<p align="center">
Total Summary 
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879908-88c318d7-1603-4395-b9b9-98685dd983c9.png"> 
</p>

<p align="center">
Lot Summary
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879906-96f066a1-09dd-4506-8c99-b50eee47ffb5.png"> 
</p>

- The design specifications MechaCar suspension coils shows variance of the suspension coils should not exceed 100 pounds psi. Manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

While the overall variance, as shown in the Total Summary data above, is under 100 psi and get within specifications, a problem with one of the individual lots comes up. Look  Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, @ 170.28.

<br>

## T-Tests on Suspension Coils

<p align="center">
    Suspension Coils Cumulative T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879911-c2cd55b4-9b8b-487d-82a6-f9fdf55e7a84.png"> 
</p>

- T-test for the suspension coils across all manufacturing lots shows that they are NOT statistically different from the mean, and the p-value is not low enough (0.0603) to reject the null hypothesis.

<p align="center">
    Suspension Coils Lot 1 T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879913-441551a5-d902-458b-b22a-07492b640d48.png"> 
</p>

- A review of the results of the T-test for the suspension coils for Lot 1 shows that they are not different from the mean, the p-value is not low enough (1) to reject the null hypothesis.

<p align="center">
    Suspension Coils Lot 2 T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879914-ecf657d1-8fea-4db3-9dba-37580fe2d7d8.png"> 
</p>

- T-test for the suspension coils for Lot 2 shows that they are not different from the mean, and the p-value is not low enough (0.6072), to reject the null hypothesis.

<p align="center">
    Suspension Coils Lot 3 T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879915-799e8148-f71d-4d1c-8fba-c2222e24d6f4.png"> 
</p>

- -test for the suspension coils for Lot 3 shows that they are slightly different from the mean, and the p-value is just low enough (0.0417) to reject the null hypothesis. This lot need to be discarded, or evaluated closer.

<br>

## Summary:

## Study Design: MechaCar vs Competition

It shows that customers tend today look for getting a car economical and reliable. That’s give more piece of mind.

</p>

#### What metric or metrics are you going to test?

<p align="center">

Comparable models for all major manufacturers on past 3 years for the following metrics:

*  Safety Feature Rating: **Independent Variable**
*  Current Price (Selling): **Dependent Variable**
*  Drive Package : **Independent Variable**
*  Engine (Electric, Hybrid, Gasoline / Conventional): **Independent Variable**
*  Resale Value: **Independent Variable**
*  Average Annual Cost of ownership (Maintenance): **Independent Variable**
*  MPG (Gasoline Efficiency): **Independent Variable**

</p>

#### What is the null hypothesis or alternative hypothesis?

<p align="center">

H<sub>0</sub>: MechaCar prototypes' average carrying capacity is similar to competitor's vehicles in the same vehicle class
H<sub>a</sub>: MechaCar prototypes' average carrying capacity is statistically above or below that of competitor vehicles.

</p>

#### What statistical test would you use to test the hypothesis? And why?

<p align="center">

Two-sample t-tests is appropriate for the hypothesis. Many samples is desirable to minimize bias and optimize accurate results. 

</p>

#### What data is needed to run the statistical test?

<p align="center">

A Multiple Linear regression is used to determine factors that have the highest possible correlation/predictability with list selling price (dependent variable); which combination has the greatest impact on price.


</p>

