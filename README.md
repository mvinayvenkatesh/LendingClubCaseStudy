# Project Name

Problem Statement:
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

The objective of this case study is to identify which variables are significant in predicting the demand for shared bikes.

Business Goal:
We have to model the demand for shared bikes with the available independent variables. It will be used to understand how exactly the demands vary with different features.


## Table of Contents
* [General Info]
* [Data Visualization]
* [Model Building]
* [Model validation]
* [Conclusion]
* [Acknowledgements]


## General Info
- Raw data provided contains data of biking
- Data contains 16 Columns and 730 Rows
- We need to analyse this data and derive linear regression model 


## Data Visualization
1. Count is high in Year (Yr) 1 which is 2019. 
2. Temp and aTemp - Resemble a linear line for cnt.
3. Casual + Registered = Cnt so we will consider Cnt in our model. so drop Casual and Registered. 
4. temp and atemp follow similar distribution. So we will use Actual Temperature (atemp).
5. There is some linearity seen above between other variables and cnt so a linear regression model can be used
6. atemp and temp are highly correlated with cnt
7. casual and registered are highly correlated with cnt which is expected since casual + registered = cnt

Categorical variable observations are given below:
1. Significant increase in cnt of bikers where weather is 1 (Clear, Few clouds, Partly cloudy, Partly cloudy)
2. Mean cnt of bikers is not significantly different during Working days or Weekdays
3. Cnt of bikers is highest during the months of 7, 8, 9 and 10th months (July – October).
4. In 2019 there is significant increase in the number of bikers (Cnt is significantly higher)
5. Season 3(Fall) the average bikers count(cnt) is significantly higher than other seasons


## Model Building
- Columns instant,dteday,temp,casual,registered were dropped. 
- Dummy variables were assigned to columns to allow better performance of model. 
- Train and test dataset was split into 70:30 ratio.
- Final model considered was using the below 12 attributes only.  
 -1 yr
 -2 atemp
 -3 windspeed
 -4 season_Spring
 -5 season_Winter
 -6 mnth_January
 -7 mnth_July
 -8 mnth_September
 -9 weekday_Saturday
 -10 weekday_Sunday
 -11 weathersit_Light Precipitation
 -12 weathersit_Mist + Cloudy

## Model validation
- Residual districution was normal
- There is no multicolinearity. This is reduced. 
- VIF of all independent variables is <5
- P Value of independent variables <0.05

## Conclusion
- R-squared is 83.3% on train set and 80.6% on test set
- Adjusted R-squared is 82.9% on train set and 79.7% on test set


## Technologies Used
- Jupyter Notebook 6.5.2
- GitHub 


## Acknowledgements
Give credit here.
- Upgrad tutorials


## Contact
Created by [@mvinayvenkatesh] - feel free to contact me!

