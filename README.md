# **Najmudin Nuwari Portfolio**
## [Project 1: Movies Analysis](https://github.com/Najmudin05/data-analysis-project-python/blob/main/Project_Movie_Analysis.ipynb)

### Project Overview 
This project utilizes a comprehensive movie dataset, developed as part of a Data Science Capstone Project, to perform exploratory data analysis (EDA). The primary goal is to uncover trends in movies based on ratings, duration, and profit, and to examine the relationships among these three aspects.

### Data Source
The data is sourced from Kaggle and contains metadata for all 45,000 movies listed in the Full MovieLens Dataset. This dataset also includes files containing 26 million ratings from 270,000 users for all 45,000 movies. Ratings are on a scale of 1-5 and were obtained from the official GroupLens website. This dataset can be accessed [here](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset).

### Data Cleaning/Preparation
In the initial data preparation phase, we performed the following tasks:
1. Understanding data
2. Data preparation (filtering and sorting data)
3. Handling duplicated and missing data
4. Feature engineering analysis

### Exploratory Data Analysis (EDA)
EDA involved exploring the movies dataset to answer key questions, such as:
1. What is the distribution of movies with a rating >3?
2. What is the distribution of the movie durations available?
3. Is there a relationship between the duration of the movie and the rating it received?
4. What is the distribution of profits generated by a movie?
5. Apakah ada hubungan antara profit dan rating?

### Results/Findings
The analysis results are summarized as follows:
1. More than 50% of the data consists of movies with a rating above 3.
2. The average movie duration is around 94 minutes.
3. Movies with good ratings mostly have durations between 90–120 minutes.
4. Only 10% of all movies make a profit.
5. Movies with good ratings do not necessarily generate large profits.
6. Movies with a rating below 3 have profits below 1 billion.

### Recommendations
Based on the analysis, we recommend the following actions:
1. Focus on quality elements like storyline and cast to improve ratings and audience satisfaction.
2. Prioritize marketing for movies with high-profit potential, especially specific genres or themes that perform well.
3. Promote lower-rated movies by bundling them with popular titles or featuring them in “hidden gems” categories.
4. Investigate genre-specific trends to better understand what drives profitability in different categories.


## [Project 2: User Retention Analysis](https://github.com/Najmudin05/data-analysis-project-python/blob/main/Project_User_Retention_Cohort.ipynb)

### Project Overview 
User retention analysis is a process used to understand whether users continue to engage with or return to use a product over time (retention). This analysis aims to identify user behavior patterns and take actions to improve retention rates, ultimately helping businesses maintain a loyal customer base. User retention analysis generally involves monitoring user activity over time to detect trends, identify engagement drivers, and understand factors contributing to user attrition.

### Data Source
This user retention analysis uses a dataset from an online retail business, containing key transaction information. The dataset includes the following columns order_id, product_code, product_name, quantity, order_date, price, and customer_id. This dataset can be accessed [here](https://github.com/Najmudin05/data-analysis-project-python/blob/main/Online%20Retail%20Data.csv)

### Data Preparation and Analysis
In the data preparation and analysis phase, we performed the following tasks:
1. Understanding data.
2. Data cleansing, create year and month columns.
3. Analyze user retention using cohort analysis 
	- Aggregate transaction data into a summary of total transactions/orders per user per month.
	- Create a column as the cohort for users, for example, the cohort of the month when they made their first transaction.
	- Calculate the month difference between the transaction month and the first transaction month, then add 1 so that a 0-month difference becomes 1, representing the first month, and so on.
	- Create a pivot table with the cohort as the index, month difference as the columns, and the values as the count of unique users (unique count of user ID).
	- Calculate the number of users in each cohort (users who made their first transaction in that month) and divide all values in the pivot table by this number according to the index row to get the retention rate.
	- Display the pivot table containing the retention rate values as a heatmap.

### Results/Findings
The analysis results are summarized as follows:
1. In January 2010, there were 713 users who made their first transaction, making it the largest cohort. This cohort also had the highest retention rate in the second month (39%), indicating a good level of continuity.
2. Additionally, this cohort remained loyal, with a retention rate of around 40% or more for the following months. However, it should be noted that the majority of users across various cohorts did not return to transact, with retention rates not reaching 50%.
3. Of particular concern is the lowest retention rate observed in December 2010, highlighting end-of-year challenges in retaining users.

### Recommendations
Based on the analysis, we recommend the following actions:
1. Launch marketing campaigns for users with lower retention rates, offering personalized reminders and promotions to bring them back.
2. Investigate why users disengage after their initial purchase to identify improvement areas in the customer experience.
3. Regularly gather user feedback to understand their needs and satisfaction levels, helping to guide product improvements.
4. Create a loyalty program that rewards repeat purchases and encourages user engagement through discounts or exclusive offers.
