RESTAURANT RATINGS ANALYSIS

Project Overview

This project analyzes restaurant data using Power BI. The project focuses on data cleaning, transformation, analysis, and dashboard creation.

Tools Used

Power BI
Power Query
DAX
Microsoft Excel
Git
GitHub

Data Cleaning

The dataset was cleaned using Power Query.

The following cleaning steps were performed:

- Removed duplicate records
- Removed unnecessary rows
- Handled missing values
- Corrected data types
- Removed extra spaces using Trim
- Removed non-printing characters using Clean
- Standardized text capitalization
- Checked invalid values
- Standardized categorical values
- Split and merged columns where required

DAX Measures

Total Restaurants

DISTINCTCOUNT(Restaurants[Restaurant_ID])


Total Records

COUNTROWS(Restaurants)


Average Rating

AVERAGE(Restaurants[Customer_Rating])


Average Owner Age

AVERAGE(Restaurants[Owner_Age])


Parking Available %

DIVIDE(
    CALCULATE(
        [Total Restaurants],
        Restaurants[Parking_Available] = "Yes"
    ),
    [Total Restaurants],
    0
)


Dashboard KPIs

Total Restaurants: 79

Total Records: 79

Average Rating: 2.98

Average Owner Age: 42.10

Parking Availability: 50.6%


Dashboard Visualizations

1. Restaurants by City

Shows the number of restaurants in each city.

2. Restaurants by Cuisine

Shows the distribution of restaurants across different cuisines.

3. Restaurants by Price Range

Shows the number of restaurants in each price category.

4. Parking Availability

Shows restaurants with and without parking.

5. Alcohol Service

Shows restaurants that provide alcohol service and those that do not.

6. Customer Rating Distribution

Groups restaurants into Poor, Average, Good, and Excellent rating categories.


Interactive Features

The dashboard contains dropdown slicers for:

City

Cuisine

Price Range

These slicers allow users to filter the entire dashboard interactively.


Key Insights

- The dataset contains 79 restaurant records.
- The average customer rating is 2.98.
- The average owner age is 42.10 years.
- 50.6% of restaurants have parking available.
- Mumbai has the highest restaurant count among the cities shown.
- Indian and South Indian cuisines have high representation in the dataset.
- High price range is the largest price category.
- Parking availability is almost evenly divided between Yes and No.
- Alcohol service is also evenly divided between Yes and No.


Project Files

Restaurant_Ratings_Analysis.pbix

Restaurant_Data_Cleaning_Practice.xlsx

README.txt


Project Skills

Power BI
Power Query
DAX
Excel
Data Cleaning
Data Analysis
Data Visualization
Git
GitHub


Project Summary

This project demonstrates the complete workflow of a beginner-level data analytics project, starting from raw and unstructured data, followed by data cleaning and transformation, DAX calculations, interactive dashboard creation, and business insights.

This project can be included in a Data Analyst portfolio to demonstrate practical skills in Power BI and data analysis.