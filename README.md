# Melbourne Housing Market Analysis

## Introduction

Welcome to the Melbourne Housing Market Analysis project. This project provides a comprehensive analysis of Melbourne's real estate market, exploring various aspects such as housing prices, sales counts, distance from the city center, building-to-land ratios, and property types. The analysis offers valuable insights into market trends, helping to inform decisions on buying or selling properties in Melbourne.

## Project Details

**Description:**  
- Rows: 34,857
- Columns: 21
- Data Types: Numerical & Categorical
- Missing Values: Included (Different imputations needed)
- Outliers: Included
- Usages: EDA, Visualization, Prediction

**Data Cleaning Results:**  
- No duplicate rows
- No columns with missing values
- No outlier values in Land Size & Building Area columns
- Number of regions: 8
- Number of council areas: 33
- Number of suburbs: 351

**Property Counts:**  
- Number of properties in each region
- Number of properties in each council area
- Top 10 suburbs with the highest number of properties

## Table of Contents

- Introduction
- Data Wrangling
- Exploratory Data Analysis
- Conclusions

## Exploratory Data Analysis Questions

### 1) What are the top 10 suburbs with the highest number of sold properties?

The figure shows the top 10 suburbs in Melbourne based on the count of property sales. Reservoir has the highest count with 510 sales, followed by Bentleigh East and Richmond with 369 and 327 sales, respectively. This indicates high demand and popularity among buyers in these suburbs.

![Top 10 Suburbs with Highest Sales Count](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q1.png){:width="400px"}

### 2) Which are the top 10 suburbs with the highest average property prices?

The figure shows the top 10 suburbs in Melbourne based on the median price of property sales. Ivanhoe East has the highest median price at 1,601,000 AUD, followed by Princes Hill and Beaumaris at 1,530,000 AUD and 1,515,000 AUD, respectively.

![Top 10 Suburbs with Highest Average Prices](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q2.png)

### 3) How do the prices and sales of modern properties compare to those of historic properties?

- Historic properties have an average price of 1,189,933 AUD, which is higher than the average price of modern properties at 964,616 AUD.
- Modern properties have a higher sales count (15,655) compared to historic properties (4,089).
- Conclusion: While historic properties may have a higher price on average, modern properties are more popular in terms of sales count.

<div style="display: flex; justify-content: center;">
    <img src="https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q3%20Price.png" alt="Price" style="width: 45%; margin-right: 5px;">
    <img src="https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q3%20Sales.png" alt="sales" style="width: 45%; margin-left: 5px;">
</div>

### 4) How does the age of a property affect its price and sales compared to modern and historic properties?

- Properties aged 49 years have the highest sales count (11,863).
- Significant drops in sales count for properties aged 59, 69, and 39 years.
- Properties aged 118, 98, and 128 years show lower sales counts but are notable outliers.
- Mid-century properties (aged 30-80 years) have the highest sales count.

<div style="display: flex; justify-content: center;">
    <img src="https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q4%20price.png" alt="Price" style="width: 45%; margin-right: 5px;">
    <img src="https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q4%20SALES.png" alt="sales" style="width: 45%; margin-left: 5px;">
</div>

### 5) Is there a correlation between the price and sales of a property regarding different regions?

- The charts show a positive correlation between the average price of properties and sales count per region.
- Regions with higher average prices also have higher sales counts.

![Average Price and Sales Count per Region](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q5%20BOTH.png)

### 6) Where should I buy a 2 bedroom unit?

- Regions with the highest average price for 2-bedroom properties are Southern Metropolitan and Eastern Metropolitan.
- These regions also have the highest overall property prices, indicating a positive correlation.

![Price of 2 Bedroom Units](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q6.png)

### 7) Is there a relationship between property prices and sales and their distance from the city center?

- Scatter plot shows a negative correlation: property prices decrease with increasing distance from the city center.
![Property Prices and Sales by Distance from City Center](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q7%20CORR%20PRICE%20PER%20DISTANCE.png)
- Bar charts show that properties closer to the city center have higher prices and sales counts.

<div style="display: flex; justify-content: center;">
    <img src="https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q7%20AVG%20PRICES%20PER%20DISTANCE.png" alt="Price" style="width: 45%; margin-right: 5px;">
    <img src="https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q7%20SALES%20AVG%20PER%20DISTANCE.png" alt="sales" style="width: 45%; margin-left: 5px;">
</div>


### 8) How do different regions compare in terms of their distance from the city center, property prices, and sales?

- Metropolitan regions closer to the city center have the highest prices, sales, and sales of 2-bedroom properties.

![Regional Comparison of Prices and Sales](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q8.png)

### 9) Is there a correlation between the distance of a property from the city center and its building to land ratio?

- Positive correlation between building to land ratio and property prices as distance to city center decreases.
- Higher building density near the city center contributes to higher property prices.

![Building to Land Ratio vs Distance](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q9.png)

### 10) How does the number of units of each housing type affect their prices, and what is the quantity and ratio of each type of unit in the area?

- Houses are the most common property type (68.4%) and have the highest average price (1,127,073 AUD).
- Units are the least expensive type but still have a relatively high count compared to townhouses.

![Property Type Count and Prices](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q10%201.png)
![Property Type Count and Prices](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q10%202.png)


### 11) What is the correlation between the number of rooms in a property and its sales count and price?

- Properties with 2, 3, and 4 rooms have the highest sales count and command some of the best average prices.
- Properties with 3 rooms have the highest sales count.

![Number of Rooms vs Sales Count and Price](https://github.com/mohamedhayaty/Melbourne-Housing-project-/blob/main/Q11.png)

## Final Conclusion

- The top 10 suburbs with the highest number of sold properties are mainly in the central and eastern parts of Melbourne.
- The top 10 suburbs with the highest average property prices are in the eastern and southeastern parts of Melbourne.
- Positive correlation between the number of rooms and sales count and price.
- Modern properties have higher sales counts, but mid-century properties (30-80 years old) have the highest sales counts overall.
- Properties closer to the city center generally have higher prices and sales.
- Houses are the most prevalent and expensive property type, while units are the most affordable.
- Different regions of Melbourne vary in distance from the city center, affecting property prices and sales.
