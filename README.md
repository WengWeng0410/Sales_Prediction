# Sales Prediction Analytic

This is a real world dataset provided during the Data Science 360 training. It is a dataset that recording the items sold (sales) based on the budget allocated for placing ads in google, facebook and instagram. Other than that, it also recording the areas and size of the market. Hence, in this project, the goal is to develop a prediction model to predict the sales of a new product based on given budget for ads, size and location of the market. 

* Perform data exploratory on the features in the data
* Develop a model to predict if the sales of a new product based on the budget allocated for google, facebook and instagram ads, and the location and size of the market

## Code and Resources Used

**Python Version:** 3.7 <br>
**Packages:** pandas, seaborn, matplotlib, sklearn <br>
**IDE:** Google Colab <br>
**Dataset:** Real world dataset provided by [360 Data Science Programm](https://thelead.io/data-science-360) by The Lead 

## Data Gathering

This is a real world dataset provided during the Data Science 360 training. It is a dataset that recording the 
* segment - ID of the record 
* google - budget allocated for placing ads in google
* facebook - budget allocated for placing ads in facebook
* instagram - budget allocated for placing ads in instagram
* sales - sales (unit sold)
* size - size of the market (large/small)
* is_large - numeric value of size feature (0 - small, 1 - large)
* area - area of the market (urban, suburban, rural)
* area_suburban - numeric value of area - suburban
* area_urban - numeric value of area - urban

## EDA

To understand the patterns and values of the data by using different types of visualizations. <br>

#### Sales Based on Budgets for Google, Facebook and Instagram Ads 
![](/images/Unit_Sold_vs_Ads.png)
Based on the graphs, it can be seen that google gives the best consistency in term of the higher the investment on ads, the higher the sales. As for facebook and instagram, the graphs are scattered, especially for invesment on instagram, where same amount of investment may give very different of sales. <br>
Google is with the better search engine, hence ads can reach to the users more accurately.

#### Sales Based on Budgets for Google, Facebook and Instagram Ads with Different Market
![](/images/Unit_Sold_vs_Ads_Size.png)
Based on the graphs, there is no significant different in term of the market size and the budget for the ads in google, facebook and facebook. Ads for both small and large markets showing sales trends that are about the same. 

#### Sales Based on Budgets for Google, Facebook and Instagram Ads with Different Area 
![](/images/Unit_Sold_vs_Ads_Area.png)
Again, similar with market size, area does not show any significant different in terms of the sales achieved based on budget allocated for the ads.

## Model Building

The input features identified for the model training are google, facebook, instagram, is_large, area_urban and area_suburban. Sales will be the output (target).
**train_test_split** from **sklearn.model_selection** is used to separat the dataset into training and testing set of data. In this project, 80% of the dataset is used as training set and the remaining 20% is used as testing set. <br>
The prediction model selected is **LinearRegression**

## Performane Evaluation

Coefficient [google, facebook, instagram, is_large, area_suburban and area_urban] and Intercept produced by the model. <br>

Coefficient:  [ 0.04574401  0.1878667  -0.0010877   0.07739661 -0.10656299  0.26813802]<br>
Intercept:  2.874190989087918 <br>

From the coefficient, it can be seen that google, facebook and area_urban play a major role in determining the unit sold (sales). <br>
As for the intercept value, it shows that there will be at least 2874 unit sold if the company did not allocate any budget for placing the ads. <br>

Based on the result, the performance of LinearRegression is good as it recoreded score of   86.32%.



















