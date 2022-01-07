# Overview of Project
                 A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:
### Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
### Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
### Run t-tests to determine if the manufacturing lots are statistically different from the mean population
### Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.
  ![Summarystatics](https://user-images.githubusercontent.com/90371048/148339902-4b87bedf-220a-46fd-8e06-02a46587d1ba.PNG)

  From the above output we can see that:
 ### The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset. 
 
 #### The p-Value for this model, p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero. 
 ###This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. Relatively speaking, his multiple regression model does predict mpg of MechaCar prototypes effectively.
![Summarystatics](https://user-images.githubusercontent.com/90371048/148506844-e50604cc-d47b-4339-b081-97e8e9d7f6e3.PNG)

 # Deliverable 2
 # Summary Statistics on Suspension Coils
 # Deliverable Requirements:  
 The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

The suspension coil’s PSI continuous variable across all manufacturing lots
The following PSI metrics for each lot: mean, median, variance, and standard deviation.

             
![Lot_summery](https://user-images.githubusercontent.com/90371048/148340939-2ffe5a65-d425-4c1f-977d-15798c89a06c.PNG)
![Lot_summery](https://user-images.githubusercontent.com/90371048/148508685-1662fe44-03e2-4de3-93e9-fa785909bdc9.PNG)
![test2](https://user-images.githubusercontent.com/90371048/148509170-55c1ea80-40e8-4d50-9a4d-b7b2ce79c283.PNG)
![test3](https://user-images.githubusercontent.com/90371048/148509247-f031ccc7-8339-477f-a9c1-e62fb6f3f86c.PNG)
![test_1](https://user-images.githubusercontent.com/90371048/148509277-6abd8b09-2cf5-469a-ac7a-42c9939ea3b8.PNG)
![plt_box2](https://user-images.githubusercontent.com/90371048/148509506-67413964-8e8e-4da7-969d-d4e294b1aab1.PNG)


