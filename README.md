# Addressing Homelessness by Improving our Understanding of Local Housing Market Factors and Homelessness' Relationship.

## Description
- The purpose of the project is to identify market factors that have established effects on homelessness, and construct and evaluate empirical models of community-level homelessness. I will be using Python and Colab to perform operations that help me towards answering the above objectives. This includes cleaning up the original data sets, analyzing the data, and using topics like regularization techniques for multiple linear regression and using tree-based methods and XGBoost.
- General conclusions that I discovered from performing the above methods consist of creating multiple linear regression models including using tree-based methods and XGBoost as well as cross validation to discover the most important market factors that have established effects on homelessness. I discovered total January precipitation, log median of rent, and proportion of one person households are the best predictors from both my additional proposal of scaling the rate of homelessness and my original proposal. This was discovered by using XGBoost for my original proposal and using a normal linear regression model for my additional proposal. A more in depth conclusion can be viewed at [Communication Presentation](https://github.com/varelandrew/Homelessness/blob/main/CommunicateTheResultsHomelessness.pdf) and [Analysis Notebook](https://github.com/varelandrew/Homelessness/blob/main/Andrew_Varela_DATA_3320_Homelessness_Analysis.ipynb)

## Requirements
- In order to complete this project I had the help from a few tools. I used Google Colab as a notebook for my code to perform my desired actions when it came to answering the question of this project. Python was my programming language of choice as it has many libraries that make plotting and cleaning up data easy. Finally, I used GitHub as my project storage as it makes it easy to link and store files that I used and created for this project.

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

## Authors
- The author of this project is Andrew Varela, a 4th year Computer Science major with a minor in Data Science currently attending Seattle University. You can find Andrew Varela on [Linkedin](https://www.linkedin.com/in/andrew-varela-a827a71b6/)

## License
- The owner of this project grants permission to use information from this repository.
