# SquirrelDATA
1. Introduction:
Dataset: 2018 Central Park Squirrel Census. Including attributes of squirrels' location, activities, age, and behavior.
Objective: Analyze the behavior patterns, geographical distributions, and relationship between the activity levels of the Squirrels.

2. Data Visualization Insights:
    1. Fur Color Distribution (Bar Plot):
      purpose: Show the distribution of primary fur colors across squirrels
      insight: For instance, gray is the most dominant color for squirrels, so we can assume that grey is more adaptive or common in Central Park
    2. Age Distribution (Pie Chart):
       purpose: Illustrate the proportion of Adult and juvenile squirrels in Central Park
       insight: Understanding age distribution could be important for the dynamics of the park. It will show us if there has been an uptake in breeding.
    3. Sighting Density Based on lat/long and Fur Color (Heatmap):
       purpose: Show squirrel sighting based on location they were found
       insight: Just to distribute the location of the squirrels can show us where they live
    4. Spacial Distribution (Scatter Plot):
       purpose: Map squirrel findings based on longitude and latitude but only in the park. So any sightings outside the park are not there
       insight: Geographical clustering can indicate preferred habitats and regions within Central Park.

3. Regression Analysis insights:
    1. Model overview and Key Findings:
       Target Variable: We defined an Activity score as the sum of all the activities that squirrels take part of. which serves as a proxyy for overall activity.
       Features: Used Y (latitude) and encoded fur color (Primary Fur COlor_cinnamon, Primacy Fur Color_gray) to understand their effects on squirrel activity.
    2. Model Findings:
       Coefficients
           1. Latitude (Y): A positive or negative coefficient indicates how location within the park affects squirrel activity levels
           2. Fur Color: The coefficients for fur color variables may suggest if certain fur colors are more or less active on average
       Model performance:
           1. R-squared: Shows how much variability in Activity Score is explained by location and fur color
           2. MAE (Mean Absolute Error): Provides a sense of the average error in predicting activity, which is useful for understanding model accuracy.
       Interpretation: The regression analysis shows correlations between locations. fur color, and activity levels. Helping to quantify the impact of each factor. For example, if squirrels in certain regions (Y values) are more active, this might point to an environmental factor influencing behavior.

4. Integrated Insights:
    1. Geographical Preferences: Both the scatter plot and regression analysis shows that location within Central Park significantly affects squirrel activity. The scatter Plot shows that the squirrels did not enter the pond in the middle of Central Park.
    2. Behavioral Trends: The Activity Score derived from multiple behavioral columns aligns with time-of-day trends shown in the visualization, confirming active periods and common behaviors.
    3. Fur Color Significance: DIstribution plots and regression coefficients collectively suggest that while fur color doesn't drastically affect behavior, certain colors may dominate specific park areas
