# Restaurant Ratings Analysis

## Project Overview

This project analyzes restaurant data using Power BI. It focuses on data cleaning, transformation, analysis, and dashboard creation.

## Tools Used

- Power BI
- Power Query
- DAX
- Microsoft Excel
- Git
- GitHub

## Data Cleaning

The dataset was cleaned using Power Query.

Cleaning steps performed:

- Removed duplicate records
- Handled missing values
- Corrected data types
- Removed extra spaces
- Removed non-printing characters
- Standardized text capitalization
- Checked invalid values
- Standardized categorical values

## Dashboard KPIs

| KPI | Value |
|---|---:|
| Total Restaurants | 79 |
| Total Records | 79 |
| Average Rating | 2.98 |
| Average Owner Age | 42.10 |
| Parking Availability | 50.6% |

## DAX Measures

### Total Restaurants

DISTINCTCOUNT(Restaurants[Restaurant_ID])

### Total Records

COUNTROWS(Restaurants)

### Average Rating

AVERAGE(Restaurants[Customer_Rating])

### Average Owner Age

AVERAGE(Restaurants[Owner_Age])

### Parking Available %

DIVIDE(
    CALCULATE(
        [Total Restaurants],
        Restaurants[Parking_Available] = "Yes"
    ),
    [Total Restaurants],
    0
)

## Dashboard Visualizations

- Restaurants by City
- Restaurants by Cuisine
- Restaurants by Price Range
- Parking Availability
- Alcohol Service
- Customer Rating Distribution

## Interactive Features

The dashboard contains dropdown slicers for:

- City
- Cuisine
- Price Range

These slicers allow users to filter the dashboard interactively.

## Key Insights

- The dataset contains 79 restaurant records.
- The average customer rating is 2.98.
- The average owner age is 42.10 years.
- 50.6% of restaurants have parking available.
- Mumbai has the highest restaurant count among the cities shown.
- Indian and South Indian cuisines have high representation in the dataset.
- High price range is the largest price category.

## Project Files

- Restaurant_Ratings_Analysis.pbix - Power BI dashboard
- Restaurant_Data_Cleaning_Practice (1).xlsx - practice dataset
- README.md - project documentation

## Skills Demonstrated

- Data Cleaning
- Data Analysis
- Power Query
- DAX
- Power BI
- Excel
- Data Visualization
- Git
- GitHub

## Project Summary

This project demonstrates a complete data analytics workflow, from data cleaning and transformation to DAX calculations, interactive dashboard creation, and insights generation.