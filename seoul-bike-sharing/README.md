# Seoul Bike Sharing Analysis

## Project Overview
In this project, I analyze rental bike data from Seoul, covering the period from December 2017 to November 2018.   

While the data may be somewhat outdated, I am using it as a practice exercise for my portfolio.  
The analytical skills demonstrated here can be applied to similar rental bike datasets, aiding in the planning and management of rental bike systems. This includes ensuring a stable supply of rental bikes, regardless of city location or time.

## Software and Tools
Python version: `Python 3.9.10`  
Python packages: `pandas`, `numpy`, `matplotlib`, `seaborn`  
Tableau: `Tableau Desktop Public Edition 2024.2.0` 

## Data Collection
The dataset is obtained from `Kaggle` [Seoul Bike Demand](https://www.kaggle.com/datasets/alishohadaee/seoul-bike-sharing-demand).  

## Data Cleaning
The dataset is in clean condition, with no `Null` values or duplicate values.  
The only change that I made to the dataset is
* convert the data type of `Date` column from `object` to `datetime64` data type.

## Data Exploration / EDA
I conducted an analysis of the dataset's numerical and categorical variables.  
The analysis is categorized into `univariate analysis`, `bivariate analysis`, `multivariate analysis` and `time series analysis`. Selected highlights from these analyses are showcased below.  
 
### Univariate Analysis
#### Distribution of rented bike count per hour
The histogram shows that the rented bike count per hour is heavily right-skewed.   
The mean value is 704.6, the median is 504.5, and the standard deviation is 645.0.  

<kbd>
<img src="https://github.com/user-attachments/assets/776a5e03-33be-4b1e-838d-789b9e12f57e">
</kbd>
 
### Bivariate Analysis
#### Rented bike count by season
The boxplot below indicates that summer has the highest rented bike count, with a median close to 1,000.   
This is followed by autumn and spring. Winter has the lowest rented bike count, with a median of less than 500.  

<kbd>
<img src="https://github.com/user-attachments/assets/b038640b-304c-45cf-a989-d53acec43a06">
</kbd>
 
### Multivariate Analysis
#### Heatmap of rented bike count by weather conditions
The heatmap below shows the correlation between the rented bike count and various weather conditions.   
The rented bike count has a positive correlation with temperature, wind speed, visibility, dew point temperature, and solar radiation. Conversely, it has a negative correlation with humidity, rainfall, and snowfall.   
However, the correlations with these weather conditions are generally weak, except for temperature, which has a moderate correlation of 0.54.   

<kbd>
<img src="https://github.com/user-attachments/assets/030621ef-514f-4e81-ba93-2032eec626a5">
</kbd>
 
### Time Series Analysis
#### Average rented bike count by hour
The line plot below shows that the average rented bike count peaks at 18:00, with a second peak at 08:00.   
This suggests high bike usage during office rush hours.  

<kbd>
 <img src="https://github.com/user-attachments/assets/cac9e37d-83b7-4744-8ee6-7a103265fe56">
</kbd>
 
#### Total rented bike count by month
The rented bike count is noticeably low from December to February, indicating a reduction in bike usage during the winter season.    

<kbd>
<img src="https://github.com/user-attachments/assets/eae80021-202b-4f41-9050-2bd10b9d54b0">
</kbd>
 
## Data Visualization
The data is visualized in an interactive Tableau dashboard, which you can explore [here](https://public.tableau.com/app/profile/lily.tiong/viz/seoul_bike_sharing/Dashboard).   
The Tableau dashboard is build from [seoul_bike_sharing.xlsx](https://github.com/ltiongl/portfolio-projects/blob/main/seoul-bike-sharing/seoul_bike_sharing.xlsx).  

<kbd>
<img src="https://github.com/user-attachments/assets/026a4f74-932b-43fc-98e8-eafdc2d964ab">
</kbd>  
  
By interacting with the moving average chart, we can gain insights into the average rented bike count over a specific period. The total bike count for that period is displayed, and the heatmap in the Tableau dashboard also reveals the total bike count under specific temperature and wind speed conditions. The rented bike count by hour for each selected condition can be viewed using the tooltip in both the heatmap and the moving average chart.  
