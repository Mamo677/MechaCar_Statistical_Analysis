                 # Overview of Project
                 A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:
    ###Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
    ###Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
    ###Run t-tests to determine if the manufacturing lots are statistically different from the mean population
    ###Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.
 > mecha_mpg <- read.csv(file="../MechaCar_mpg.csv",check.names=F,stringsAsFactors = F) 
> lm(mpg ~ vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD, data=mecha_mpg)

Call:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance + AWD, data = mecha_mpg)

Coefficients:
     (Intercept)    vehicle_length    vehicle_weight     spoiler_angle  
      -1.040e+02         6.267e+00         1.245e-03         6.877e-02  
ground_clearance               AWD  
       3.546e+00        -3.411e+00  

> summary(lm(mpg ~ vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD, data=mecha_mpg)) 

Call:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance + AWD, data = mecha_mpg)

Residuals:
     Min       1Q   Median       3Q      Max 
-19.4701  -4.4994  -0.0692   5.4433  18.5849 

Coefficients:
                   Estimate Std. Error t value Pr(>|t|)    
(Intercept)      -1.040e+02  1.585e+01  -6.559 5.08e-08 ***
vehicle_length    6.267e+00  6.553e-01   9.563 2.60e-12 ***
vehicle_weight    1.245e-03  6.890e-04   1.807   0.0776 .  
spoiler_angle     6.877e-02  6.653e-02   1.034   0.3069    
ground_clearance  3.546e+00  5.412e-01   6.551 5.21e-08 ***
AWD              -3.411e+00  2.535e+00  -1.346   0.1852    
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 8.774 on 44 degrees of freedom
Multiple R-squared:  0.7149,	Adjusted R-squared:  0.6825 
F-statistic: 22.07 on 5 and 44 DF,  p-value: 5.35e-11

> lm(mpg ~ vehicle_length + ground_clearance, data=mecha_mpg)

Call:
lm(formula = mpg ~ vehicle_length + ground_clearance, data = mecha_mpg)

Coefficients:
     (Intercept)    vehicle_length  ground_clearance  
         -91.557             6.081             3.567  

> summary(lm(mpg ~ vehicle_length + ground_clearance, data=mecha_mpg)) 

Call:
lm(formula = mpg ~ vehicle_length + ground_clearance, data = mecha_mpg)

Residuals:
    Min      1Q  Median      3Q     Max 
-17.493  -7.705   1.344   6.642  18.500 

Coefficients:
                 Estimate Std. Error t value Pr(>|t|)    
(Intercept)      -91.5573    13.9649  -6.556 3.86e-08 ***
vehicle_length     6.0811     0.6732   9.033 7.68e-12 ***
ground_clearance   3.5669     0.5401   6.604 3.26e-08 ***
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 9.078 on 47 degrees of freedom
Multiple R-squared:  0.674,	Adjusted R-squared:  0.6601 
F-statistic: 48.59 on 2 and 47 DF,  p-value: 3.637e-12
   
    
