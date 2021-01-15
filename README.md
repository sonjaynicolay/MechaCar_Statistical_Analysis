![Mecha Image](Mecha_Image.jpg)


# MechaCar Statistical Analysis
***

## Linear Regression to Predict MPG


* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?


Vehicle Length and Ground Clearance provided a non-random variance to the mpg values. Their p-values were significantly less than .05. 



* Is the slope of the linear model considered to be zero? Why or why not?


The slope is not considered to be zero, the independent variables did appear to eefect the dependent variable causing a slope. 



* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?


This particular linear model is considered to predict MPG of MechaCar prototypes. By observing the R-Squared value or .7149. we are able to determine that the model will predict the MPG of MechaCar prototypes correctly between 71-72% of the time.


***
## Summary Statistics on Suspension Coils


In this section of the analysis I took a look at the total summary of suspension coil dataset. After getting the total summary I split the data by the  three lot numbers, to create a lot summary. This allows for a further analysis is possible variation in manufacturing and other contributing factors.


#### Total Summary

![Total Summary](Images/Total_Summary_image.jpg)

#### Lot Summary

![Lot Summary](Images/Lot_Summary_image.jpg)


* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?


At this time there is some discrepency with the data from Lot 3. As we can see the variance is more than double the total summary amount. At this time Lot 1 and Lot 2 meet the design specifications. The total summary is also within range. It would be best to use scrap Lot 3.


***

## T-Tests on Suspension Coils


Using the t.test() and its subset() argument function, I wrote and ran 4 T-test to determine if the PSI across all manufacturing lots were statistically different from the population mean of 1,500 pounds per square inch.

Looking at the test and results below the PSI across all manufacturing lots were not significantly statistically different.


![T Test 1](Images/t_test_1.jpg)

![T Test 2](Images/t_test_2.jpg)

![T Test 3](Images/t_test_3.jpg)

![T Test 4](Images/t_test_4.jpg)


***
## Study Design: MechaCar vs Competition




* What metric or metrics are you going to test?

In a statistical study that could quantify how MechaCar performs against the competitition I would include safety rating, maintenance cost and city fuel efficiency in family vehicles and larger models. In smaller, faster models I would focus on and probably emphasis highway fuel efficiency, horse power and cost. 



* What is the null hypothesis or alternative hypothesis?
Vehicles with lower horse power have a better saftety rating.



* What statistical test would you use to test the hypothesis? And why?
I believe I would use an ANOVA test for safety rating and horse power and look at ways to breakdown the types of vehicles (family versus sports models).

I may also take a look at the possibilities of running mulitple others tests to see the links and variance between classification of hybrid models. 



* What data is needed to run the statistical test?
I would need safety rating data as well as vehicle stats, that list engine specs & vehciles descriptions, etc.
