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
- Google sheet (for querying and analysis)
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

- I utilized Google Query to query the dataset ensuring that the data can answer the some questions about the data such as: 
  - Query to analyze sales performance by sales reps within each region for the years 2014 and 2015.
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
    
### Exploratory Data Ananlsis (EDA)
---
The Exploratory Data Analysis (EDA) which involve exploring the Data to answer some questions about the Data gave more insight such as:

- I showed total number of regions and the region with the highest sales

  ![visuals 1](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/22fd15c3-5165-4036-9d46-0fad9f15eac8)
  
- I showed the year that had the highest sales

![assignment 8](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/5d443eeb-8290-459e-a9a8-5df98a5f6dd7)

I showed the following:
  - Total disticnt number of Sales_rep  
  - Total distinct number of items sold
  - Which item(s) is/are topsellers
  - Which item sold highest by percentage
  - Overall sales trend
  - Total sales
  - Sales per month

![visuals](https://github.com/DebComet/SkilHarvest_Crash_Course/assets/158510031/9f4b51ab-1875-4e32-a9ef-315fee8ea042)


### Data Analysis

I included some basic lines of code, queries and DAX expressions during my analysis. They include:

`=QUERY(A:H, "SELECT MIN(H))", 1)`

`=QUERY(A:H, "SELECT MAX(H)", 1)`

`=QUERY(A:H, "SELECT AVG(H)", 1)`

`=QUERY(A:H, "SELECT C,F,H WHERE (C= 'Binder' OR C= 'Pencil') AND F=2015", 1)`

`=QUERY(A:H, "SELECT A,F,H WHERE (A= 'Central' OR A= 'East') AND F=2014", 1)`

`=QUERY(A:H, "SELECT E,F,H WHERE (E= 'Aug' OR E= 'Sep') AND F= 2014", 1)`

### Results / Findings

Insight gotten from the analysis include:
  - **Sales Performance Trends**: The analysis reveals decrease in sales volumes between 2014 and 2015.

  - **Regional Disparities**: By comparing sales the data across the three regions, I identified disparities in sales performance which include variations in quantities sold, customer 
      acquisition rates between regions.

  - **Top Performing Sales Reps**: The dataset highlights top-performing sales representatives within the region with the highest sales based on metrics such as total sales revenue, 
      sales growth.

  - **Product Performance**: The analysis of item sales data reveal insights into the popularity and demand for different stationary supplies in 2014 and gadually declined as the year 
      progessed. This could help identify best-selling item, region, and emerging trends in consumer preferences.

  - **Identification of Opportunities and Challenges**: My analysis predicts uncovered opportunities for growth, expansion, or optimization within regions where less sales were made 
      (East and West). Likewise, the challenges or obstacles to sales success, like competitive pressures, economic factors, and/or logistical issues, could be identified.


### Recommendations

 1. Plan strategic sales based on region: Sales strategies based on the performance of each region should be made as gathered from the dataset. Identifying and capitalizing on regional 
    preferences, market trends, and customer behaviors are paramount to optimize sales efforts.

 2. Training and Development: Targeted training and development programs should be offered for sales representatives to enhance their skills and effectiveness. Focusing on areas where 
    performance may be lacking or where improvement opportunities have been identified through data analysis.

3. Incentive Programs: Implement incentive programs (such as bonuses, rewards, or recognition for top-performing reps) should be considered to motivate sales representatives and drive 
   performance, especially to those who consistently exceed sales targets or demonstrate exceptional performance.

 4. Product Portfolio Optimization: The need to review product portfolio based on sales data cannot be overemphasized. This  is to identify high-demand items and underperforming item 
    which would help in organizational decision to discontinue or reposition low-performing items and rather invest resources in promoting and expanding the sales of popular items.

 5. Cross-Regional Collaboration: Collaboration and knowledge sharing among sales teams across different regions needs be encouraged. Exchange of best practices, successful sales 
    strategies, and lessons learned can drive overall sales performance improvement.

 6. Competitive Analysis: Competitive analysis to benchmark performance against competitors operating within the same regions can be done. This will help identify competitive strengths 
    and weaknesses, and develop strategies to gain a competitive edge in the market.

 7. Continuous Monitoring and Evaluation: Ongoing monitoring and evaluation of sales performance metrics mechanism houd be estabished to regularly review and analyze sales data, track 
    progress, identify emerging trends, and make informed adjustments to sales strategies and tactics as needed.


### Limitations

The limitations to my analysis are:
  1. Limited Time Frame: The dataset only covers sales data from the years 2014 to 2015. This limited time frame may not capture long-term trends or seasonal variations that could 
     influence sales performance.

  2. Scope of Analysis: The dataset focuses specifically on sales data and may not include other relevant factors that could impact sales performance, such as marketing efforts, 
     economic conditions, competitor activity, or changes in consumer preferences.

  3. Regional Variations: While the dataset covers three regions, there may be significant differences in market dynamics, customer behavior, and competitive landscapes within each 
     region. Failing to account for these variations could limit the effectiveness of region-specific recommendations.

  4. Assumptions and Interpretations: Any analysis conducted on the dataset relies on certain assumptions and interpretations of the data. It's essential to acknowledge and validate 
     these assumptions to ensure the reliability and validity of the analysis results.

  5. External Factors: External factors beyond the dataset's scope, such as changes in market regulations, technological advancements, or unforeseen events (e.g., natural disasters, 
     economic downturns), could influence sales performance but may not be captured in the analysis.

  6. Data Privacy and Security: As a result of the nature of the dataset, there were some limitations in ensuring data security as per data protection regulations and confidentiality of 
     sensitive information.

  7. Sampling bias which occurs when the method used to collect a sample from a population systematically favors certain individuals or groups over others. In this analysis, the dataset 
     being analyzed does not accurately represent the entire population it's meant to represent thereby resulting to a limitation.



