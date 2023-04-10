# AgroSapiens
Market Analysis for Farmers(Somewhat on similar mechanism as of Stock Market predictor ML)

This was Created as a part of a hackathon (National Agro Hackathon organised by LNCT and Horticulture Dept. of M.P. Gov.) 

# DATA SET 
ICRISAT (http://data.icrisat.org/dld/src/visualization.html)<for pricing of crops> and FAOSTAT(https://www.fao.org/faostat/en/)<for macro economics indicator and some other stuff as well>

# WORKING 
  so it is basically divide into three modules out of which 2 are uploaded here

## MODULE 1 : **Market Analysis** 
Here i have imported required libraries that are used while implementing a machine learning model
i have first created a data frame. Then have dropped out several factors assuming them to be 
constant so that it is easy to work with and then i have divided the dataset into training dataset, testing dataset and validation dataset

now at this point of time i have visualized the dataset which is usually the first thing that is done but its fine to do it here as we have removed
redundancy. Now i have defined the target field as Y and the remaining fields as X

### *LINEAR REGRESSION MODEL*
With this being done now finally i have implemented the linear regression method and trained my model on it
later i have evaluated its performance with metrics such as mse and all which came out to be around 0.685

after this i have also included the dataset for GDP based on agriculture of various years for india given by UN(Food and Agriculture Organization (FAO))
this helped the model to draw more precise calculations.same is done by inculding one more feature column that goes like VAAFF(value added on gdp by Agriculture,Forestry and Fishery).

by adding these two feature vectors the score increased from 0.685 to .90899
for more better accuracy and predictions i tried to use random forest regression model

### *RANDOM FOREST REGRESSION*
as we already had the training dataset and everything set up
therefore all i did is passsed that data and got the score as  0.98424

and thats it for the 1st module.
