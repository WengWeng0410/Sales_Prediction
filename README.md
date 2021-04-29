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



















