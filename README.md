# MechaCar_Statistical_Analysis_R_Practice_

## Linear Regression to Predict MPG


Inpependent Variables: vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD

![image](https://user-images.githubusercontent.com/99847046/209764665-8c8b397e-06fc-48f3-8bbf-c2a4d68138c4.png)


### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Based on the results Vehicle_length and ground clearance are very unlikely to provide random amounts of variance in the linear model.  So these independent 
variables are should be considered as having a strong influence on the MPG of the vehicle.

### Is the slope of the linear model considered to be zero? Why or why not?

The linear model would not be considered zero as the p-value from the summary is less than a normal significant value of 0.05.


### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

At first glance, I don't believe it does because of the value of the Intercept.  Our intercept is statistically significant, so the inpendent variables we determined to be significant features may need scaling to improve prediction value of the model.  However the Multiple R-squared value indicates 71% of the variability of MPG is explained by this model. A bonus thought is vehicle_weight should have a significant influence on mpg based on intuition but according to this model it does not. 




##Summary Statistics on Suspension Coils

Let's say the design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 PSI. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![image](https://user-images.githubusercontent.com/99847046/209764975-4e78ea35-70b8-422b-99d2-7c36bba6e118.png)

When data from all lots are summarized, the variance is well within 100 PSI, meeting design specification requirments. 

![image](https://user-images.githubusercontent.com/99847046/209765003-b346c5d2-a35b-4622-a273-075ace8fe412.png)

However, when grouped into different lots, LOT 3 has significant deviation from the mean. 



