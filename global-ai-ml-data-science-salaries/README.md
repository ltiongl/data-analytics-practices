# Global AI, ML, and Data Science Salaries Analysis

## Project Overview
This project explores global salary trends in AI, ML, and data science from 2020 to 2024. The data includes information on job titles, experience levels, employment types, salaries, employee residences, remote work ratios, company locations, and company sizes.  

## Software and Tools
Python version: `Python 3.9.10`  
Python packages: `pandas`, `numpy`, `matplotlib`, `seaborn`  
Tableau: `Tableau Desktop Public Edition 2024.2.0` 

## Data Collection
The dataset is obtained from `Kaggle` [Global AI, ML, and Data Science Salaries](https://www.kaggle.com/datasets/msjahid/global-ai-ml-and-data-science-salaries).  

## Data Cleaning
The dataset contains no Null values but has 16,646 duplicate entries. These duplicates were left intact, as it’s possible for identical data to represent different cases, so no action was required.  
  
For data cleanup:   
1. Abbreviations and numeric codes were updated to descriptive words for easier readability. 
* `experiment_level`
  * `EN`: `Entry-level / Junior`
  * `MI`: `Mid-level / Intermediate`
  * `SE`: `Senior-level / Expert`
  * `EX`: `Executive-level / Director` 
* `employment_type`
  * `PT`: `Part-time`
    `FT`: `Full-time`
    `CT`: `Contract`
    `FL`: `Freelance`
* `remote_ratio`
  * `0`: `No remote work`
  * `1`: `Partially remote / hybrid`
  * `100`: `Fully remote`
* `company_size`
  * `S`: `less than 50 employees`
  * `M`: `50 to 250 employees`
  * `L`: `more than 250 employees`
2. Update data types.
* `work_year`
  * convert the data type of `Date` column from `object` to `datetime64` data type

## Data Exploration / EDA
I conducted an analysis of the dataset's numerical and categorical variables.  
The analysis is categorized into `univariate analysis`, `bivariate analysis` and `time series analysis`. Selected highlights from these analyses are showcased below.  
 
### Univariate Analysis
#### Distribution of annual salary
The histogram shows that most annual salaries fall within the range of 100,000 to 200,000 USD.   

![image](https://github.com/user-attachments/assets/8721a3b0-cb92-4a25-a4ce-d11c7e6225bd)

The statistics summary of salary:
* mean: 159,188 USD
* median: 149,800 USD
* mode: 150,000 USD

#### Top 10 job ranking
The data provides insights into the top 10 job titles in AI, ML, and data science.  

![image](https://github.com/user-attachments/assets/81ffe7de-e79f-4a60-b0b8-e979d59a5212)

### Bivariate Analysis
#### Salary by employment type
The boxplot shows that full-time positions have the highest average annual salary, followed by contract and part-time roles. Freelance positions have the lowest salaries. The salary range within each employment type is relatively narrow.   

![image](https://github.com/user-attachments/assets/b98830ba-8c8d-46fd-9d34-4c3350b97078)

### Time Series Analysis
#### Top 10 job title count by year
The data shows that the number of data scientist positions has more than doubled each year. Data engineer roles have grown at a similar rate, but by 2024, data scientist positions outnumber data engineer roles by approximately 1,000. Software engineer and machine learning engineer job counts have remained similar, with both increasing at the same rate.

![image](https://github.com/user-attachments/assets/4373fa81-6081-45ea-bf88-68fa67023d4a)


## Data Visualization
The data is visualized in an interactive Tableau dashboard, which you can explore [here](https://public.tableau.com/app/profile/lily.tiong/viz/global_ai_ml_data_science_slaaries/Dashboard).   
The Tableau dashboard is build from [global_ai_ml_data_science_salaries.xlsx](https://github.com/ltiongl/portfolio-projects/blob/main/global-ai-ml-data-science-salaries/global_ai_ml_data_science_salaries.xlsx).  

![image](https://github.com/user-attachments/assets/a2ec3cc2-baa4-45f2-b547-29152c126bde)

The dashboard features charts displaying the average salary by year, categorized by experience level and the top 10 employee residences. It also includes pie charts for company size, experience level, and employment type. Additionally, there’s a map showing average salaries by country and a scatter plot for average salary by experience level and employment type. The control panel allows for filtering by company location, job title, and work year.  
