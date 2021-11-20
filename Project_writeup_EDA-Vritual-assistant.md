# Analysis of the Saudi market in vehicles
Bushra yousif 

## Abstract
The goal of this project was to use classification models to predict the operating condition of waterpoints in Tanzania in order to help improve operations and maintenance planning of these units. I worked with data provided by [Taarifa](http://taarifa.org/) and the Tanzanian Ministry of Water, leveraging geographic and categorical feature engineering along with a random forest model to achieve promising results for this multiclass problem. After refining a model, I built an interactive dashboard to visualize and communicate my results using Tableau.      

## Design
This project originates from the [DrivenData competition](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/) "Pump it Up: Data Mining the Water Table". The data is provided by [Taarifa](http://taarifa.org/) and the Tanzanian Ministry of Water, and presents a three-class operational status of **functional**, **functional needs repair**, and **non-functional** for waterpoints across the country. Classifying statuses accurately via machine learning models would enable the Tanzanian Ministry of Water to take action to improve operations and maintenance planning of these units, allocate resources more quickly to needed areas, and ensure potable water is accessible to as many people as possible.

## Data
The dataset contains 59,400 waterpoints with 40 features for each, 32 of which are categorical. A few feature highlights include measurements of water quantity and quality, pump types, and latitude/longitude coordinates. Nearly a third of the individual features could be grouped into more general categories, and an in-depth analysis of 20 of them was undertaken to inform baseline models and feature engineering. 

## Algorithms

*Feature Engineering*
1. Mapping latitude and longitude to 3-dimensional coordinates so nearby continuous values would also be close in reality
2. Converting categorical features to binary dummy variables
3. Combining particular dummies and ranges of numeric features to highlight strong signals and illogical values for waterpoint status identified during EDA
4. Selecting subsets of the total unique values for categorical features that were converted to dummies, according to the number of samples they were associated with and their contribution to certain statuses


## Tools
- Numpy and Pandas for data manipulation
- Matplotlib and Seaborn for plotting
