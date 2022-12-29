# MechaCar_Statistical_Analysis_R_Practice_

## Linear Regression to Predict MPG


Inpependent Variables: vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD

![image](https://user-images.githubusercontent.com/99847046/209764665-8c8b397e-06fc-48f3-8bbf-c2a4d68138c4.png)


### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Based on the results Vehicle_length and ground clearance are very unlikely to provide random amounts of variance in the linear model.  So these independent 
variables are should be considered as having a strong influence on the MPG of the vehicle.  Using AVplots backs this up with Vehicle_length and ground clearance steaper lines than the other variables.

![image](https://user-images.githubusercontent.com/99847046/209767487-087f8877-d295-4576-bcf9-bb9659a01500.png)


### Is the slope of the linear model considered to be zero? Why or why not?

The linear model would not be considered zero as the p-value from the summary is less than a normal significant value of 0.05.


### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

At first glance, I don't believe it does because of the value of the Intercept.  Our intercept is statistically significant, so the inpendent variables we determined to be significant features may need scaling to improve prediction value of the model.  However the Multiple R-squared value indicates 71% of the variability of MPG is explained by this model. A bonus thought is vehicle_weight should have a significant influence on mpg based on intuition but according to this model it does not. 




## Summary Statistics on Suspension Coils

## Let's say the design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 PSI. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![image](https://user-images.githubusercontent.com/99847046/209764975-4e78ea35-70b8-422b-99d2-7c36bba6e118.png)

When data from all lots are summarized, the variance is well within 100 PSI, meeting design specification requirments. 

![image](https://user-images.githubusercontent.com/99847046/209765003-b346c5d2-a35b-4622-a273-075ace8fe412.png)

However, when grouped into different lots, LOT 3 has significant deviation from the mean. 


## T-TEST of PSI 

We want to know if the mean for the PSI variable from the Suspension Coil table is statistically different from a population mean of 1500 PSI.

All Lots
![image](https://user-images.githubusercontent.com/99847046/209899336-3b5e09db-d8e6-4edf-a919-f550a1d7c408.png)
  
The P-value is greater than the significance level of 0.05.  Which means we fail to reject the null hypothesis the both the sample mean and population are
statistically similar.
  
Lot 1
![image](https://user-images.githubusercontent.com/99847046/209899793-adac41e5-7786-4340-8f23-d941d03f1037.png)

Fail to reject the Null Hypothesis.

Lot2
![image](https://user-images.githubusercontent.com/99847046/209899818-18c60b74-f016-47e6-afd0-8f85f3061877.png)

Fail to reject the Null Hypothesis.

Lot3
![image](https://user-images.githubusercontent.com/99847046/209899832-eb9f555a-4584-4de4-80c5-a6b4d584a882.png)

For Lot 3 however, we reject the null hypothesis because the P-value is greater than 0.05.  The conclusion here is than the two means 
are statiscally different.






