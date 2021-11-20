# Analysis of the Saudi market in vehicles
Bushra yousif 

## Abstract
The goal of this project was to explore most used cars of the Saudi market and utilize data set to recommend used vehicles in order to help women's empowerment and make clear list of the most-best used carso they can get/view the list without wasting time. I worked with data provided by [kaggle](https://www.kaggle.com/reemalruqi/used-cars-in-saudi-arabia) and Yallamotor is website in ksa have a collection of used vehicles for sale.

## Design
This project originates for virtual assistant for women's empowerment based on clean , design and visualize all of client backstory requests
[Client request](Client request for best-most used car in SA.md)


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
