# SkilHarvest_Stationary_Supplies

Here, I documented all I learnt and practiced during my course at SkilHarvest_Bootcamp.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Data Source](#data-source)
3. [Tools Used](#tools-used)
4. [Data Cleaning and Preparation](#data-cleaning-and-preparation)
5. [Exploratory Data Analysis](#exploratory-data-analysis)
6. [Data Analysis](#data-analysis)
7. [Results / Findings](#results-/-findings)
8. [Recommendations](#recommendations)
9. [Limitations](#limitations)

### Project Overview
---
The Stationary Supplies Dataset covers sales data from the years 2014 to 2015, providing valuable insights into the performance of Sales reps within three regions.

This analysis was done with the aid of Googlesheets (which is a web-based spreadsheet application developed for its productivity within Google Drive. It provides a powerful and user-friendly platform for creating, editing, and collaborating on spreadsheets, making it a popular choice for individuals, teams, and organizations).

It was queried using google query (a powerful feature within Google Sheets that provides a flexible and efficient way to analyze and manipulate data within Google Sheets, making it a valuable tool for data analysis, reporting, and visualization).

### Data Source
---
The Stationary Supplies Dataset utilized in this analysis encompasses sales data from the years 2014 to 2015. This dataset was sourced from 'Skilharvest_Stationary_Supplies.csv', a reputable provider of comprehensive datasets in the retail industry.

### Tools Used
---
- MS Excel for Data Cleaning [Download Here](https:/www.microsoft.com)
- Google sheet (for Querying and analysis)
- Power BI (for reporting)
- MS Powerpoint (for presentation)

### Data Cleaning and Preparation
---
- I imported the dataset into Google Sheets.

![stationary dataset](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/42a1d2b3-7664-4862-86ab-51b62117d211)

- I ensured that the dataset included sales data within  2014 and 2015 and covers information about sales reps within three regions.

The data, on observation had no missing values, irrelevant columns, duplicate rows or inconsistencies.

- I edited the dataset to allow the first row of my dataset become header. 
- Ensure that data columns are labeled clearly and consistently for easy reference during analysis.


### Exploratory Data Analysis
---
- I utilize Google Query to query the dataset within Google Sheets.
  - I wrote queries to analyze sales performance by sales reps within each region for the years 2014 and 2015.
    1. **Sales of Bnder and Pencil in 2015**

       `=QUERY(A:H, "SELECT C,F,H WHERE (C= 'Binder' OR C= 'Pencil') AND F=2015", 1)`
       
     ![assignment 1](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/8e6961a9-6641-41e6-a7ee-0927e841d5c4)

    2. **Sales in Central and East regions in 2014**

       `=QUERY(A:H, "SELECT A,F,H WHERE (A= 'Central' OR A= 'East') AND F=2014", 1)`

      ![assignment 2 pics](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/c44dbb8f-5214-40e2-a06f-9298cd7a1fba)
    
    3. **Sales in August and September 2014**

       `=QUERY(A:H, "SELECT E,F,H WHERE (E= 'Aug' OR E= 'Sep') AND F= 2014", 1)`

      ![assignment 3 pics](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/1c74bb29-723a-452c-9014-78ee943e0d46)
    
    4. **Sales of items whose name(s) start with 'Pen', the sales rep, region(s) and year**

       `=QUERY(A:H, "SELECT A,B,C,F,H WHERE (C LIKE 'Pen%') AND F= 2014", 1)`

      ![assignment 4 pics](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/08cc6529-8e6b-4c35-9175-3c5978e22dad)

    5. **Query the sales rep who sold Pen set and Binder**

       `=QUERY(A:H, "SELECT B, C WHERE (C= 'Pen Set' OR C= 'Binders')", 1)`

       ![new assignment 5](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/62b55f96-c8a3-406b-b480-914f31fdc72d)

    6. **Query the minimum, maximum, average, count and total sales**

    ![assignment 6](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/5f57bac9-6439-4dd0-97b2-1334ca0a5d1b)   
    
       
Use SQL-like syntax to filter, aggregate, and manipulate the data as needed to derive insights.
Analysis and Visualization:

Perform data analysis using the queried results to identify trends, patterns, and outliers in sales performance.
Create visualizations such as charts, graphs, and pivot tables to visualize the analyzed data and present key findings.
Utilize Google Sheets' built-in functions and features for data analysis and visualization.
Documentation and Reporting:

Document the data cleaning, preparation, querying, and analysis process for future reference.
Prepare a summary report or presentation using Google Docs or Google Slides to communicate the key findings and insights derived from the analysis.
Share the report with relevant stakeholders or team members for review and feedback.
By following these steps, you can effectively clean, prepare, query, analyze, and visualize the Stationary Supplies Dataset using Google Sheets and Google Query to derive valuable insights into sales performance across different regions and years.

### Exploratory Data Ananlsis (EDA)
---
The Exploratory Data Analysis (EDA) involved exploring the Data to answer some questions about the Data such as:
- Total number of Sales_rep
- The region from where most Sales_reps resided
- Total number of regions
- Which region had the highest sales
- Total number of items sold
- Which item(s) is/are topsellers
- Which Sales_rep made the highest sales
- Which year was the highest sales made
- Overall sales trend
- Minimum, Maximum, Average and Count of sales


![](assignment1.JPG)


```Google sheets

SELECT *
From Table 1
WHERE H = Positive integers

```









