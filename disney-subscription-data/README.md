# Disney+ Subscription Data Analysis

## Project Overview
Using Disney+ subscription data, I analyzed monthly revenue and subscriber demographics.  

## Software and Tools
Python version: `Python 3.9.10`  
Python packages: `pandas`, `numpy`, `matplotlib`, `seaborn`  
Tableau: `Tableau Desktop Public Edition 2024.2.0` 

## Data Collection
The dataset is obtained from `Kaggle` [Subscription Data Disney+](https://www.kaggle.com/datasets/albeyee/subscription-data-disney).  

## Data Cleaning
The dataset is in clean condition, with no `Null` values or duplicate values.  
Changes for data cleaning:  
* convert `Plan Duration` data in Year and Month to only Month.
* convert the data type of `Plan Duration` column from `object` to `int` data type.

## Data Exploration / EDA
The `Monthly Revenue` data is not listed out for each month within the plan duration. Only basic univariate analysis was conducted in Python. The data is reorganized to create a new table listing `Monthly Revenue` for each subscription month. Detailed data exploration will be carried out in Tableau.  
 
### Univariate Analysis
#### Distribution of subscribers by age
The count plot displays the distribution of subscribers by age.  
There is no clear trend in the distribution of subscribers' ages.  

![image](https://github.com/user-attachments/assets/a73b0b4b-bc7f-410b-a870-758c97028dd0)

#### Count plot of plan duration
The plot below shows that most subscribers opt for a 24-month subscription, followed by a 1-month plan as the second most common duration.

![image](https://github.com/user-attachments/assets/442baf10-8f50-4a0d-963c-5e6269b295b3)

## Data Visualization
The data is visualized in an interactive Tableau dashboard, which you can explore [here](https://public.tableau.com/app/profile/lily.tiong/viz/disney_subscription_data/Dashboard).   
The Tableau dashboard is build from [disney_subscription_data_final.xlsx](https://github.com/ltiongl/portfolio-projects/blob/main/disney-subscription-data/disney_subscription_data_final.xlsx) and [disney_subscription_data_final_revenue.xlsx](https://github.com/ltiongl/portfolio-projects/blob/main/disney-subscription-data/disney_subscription_data_final_revenue.xlsx).  

![image](https://github.com/user-attachments/assets/10346013-0035-46bb-b3fa-af99bf814867)

By using the Date by Month control panel, you can view the monthly revenue from Disney+ subscriptions, calculated based on actual subscriber payments. The dashboard also displays the distribution of subscribers by country, with the majority coming from the United States. Additionally, you can analyze subscriber counts by gender and age range for specific time periods.  
