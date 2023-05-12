# Addressing Homelessness by Improving our Understanding of Local Housing Market Factors and Homelessness' Relationship.

## Description
- The purpose of the project is to identify market factors that have estabished effects on homelessness, and construct and evaluate empirical models of community-level homelessness. I will be using Python and Colab to perform operations that help me towards answering the above objectives. This includes cleaning up the original data sets, analyzing the data, and using topics like regularization techniques for multiple linear regression and using tree-based methods and XGBoost.

## Data
- The dataset consists of various housing, economic, safety net, demographic, and climate factors sourced largely from HUD and U.S. Census Bureau databases. If you want a more in-depth look into the source of the data look here: [Market Predictors of Homelessness](https://www.huduser.gov/portal/sites/default/files/pdf/Market-Predictors-of-Homelessness.pdf).
- I gathered one dataset and a dictionary describing the variables in the dataset that reflect the above description: [Data Set](https://github.com/varelandrew/Homelessness/blob/main/HUD%20TO3%20-%2005b%20Analysis%20File%20-%20Data%20-%20Dictionary.csv) and the other can be found here: [Dictionary](https://github.com/varelandrew/Homelessness/blob/main/05b_analysis_file_update.csv)

## Data Preparation
- What steps did I take to prepare a cleaned up version of the data sets from the websites above?
1. I first imported necessary libraries and loaded the dataset and dictionary.
2. I then explored the contents of both the dataset and dictionary to see what I was working with and what needed to be cleaned up.
3. First thing I noticed is the mass amount of columns inside the dataset. I created a subset of columns that I thought would be useful in the future and updated the dataset to reflect those columns.
4. Once I updated the dataset I renamed the columns to reflect to follow good format consisting of lowercase, snake_case, readable variables.
5. Then I identified missing values and ended up dropping nan values from total_homeless and dropping all rows that weren't from 2017.
6. Lastly, I converted columns that consisted of some total of a group and made them into a percentage by every 10,000 people compared to the total_population.
7. Then I exported the clean data set.
- Here you can find the python file that follows these steps I listed: [Data Preparation File](https://github.com/varelandrew/Homelessness/blob/main/Andrew_Varela_DATA_3320_Homelessness_Data_Preparation_Template.ipynb)
- Here you can find the cleaned csv file: [Clean Data](https://github.com/varelandrew/Homelessness/blob/main/clean_homeless.csv)
