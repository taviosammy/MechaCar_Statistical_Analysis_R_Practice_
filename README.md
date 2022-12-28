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

At first glance I don't believe it does because of the value of the Intercept.  Our intercept is statistically significant, so the inpendent variables we determined to be significant features may need scaling to improve prediction value of the model.  However the Multiple R-squared value indicates 71% of the variability of MPG is explained by this model. A bonus thought is vehicle_weight should have a significant influence on mpg based on intuition but acording to this model it does not. 
