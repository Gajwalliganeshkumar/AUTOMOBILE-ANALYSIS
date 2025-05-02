#  Automobile Dataset - Exploratory Data Analysis (EDA)

##  Project Overview

This project performs in-depth Exploratory Data Analysis (EDA) on an automobile dataset consisting of 11,000+ records and 16 features. The analysis includes identifying and treating missing values, duplicate entries, outliers, and generating insightful visualizations to better understand car features such as mileage, price, fuel type, and more.


##  Dataset Features

| Feature              | Description                             |
|----------------------|-----------------------------------------|
| `Make`               | Manufacturer name                       |
| `Model`              | Car model                               |
| `Year`               | Model release year                      |
| `Fuel Type`          | Type of fuel used                       |
| `Horse Power`        | Engine power                            |
| `Cylinders`          | Number of engine cylinders              |
| `Transmission Type`  | Type of transmission                    |
| `Driven_Wheels`      | Drive system                            |
| `Number of Doors`    | Number of doors                         |
| `Market Category`    | Vehicle's marketing classification      |
| `Vehicle Size`       | Compact, Midsize, or Large              |
| `Vehicle Style`      | Sedan, SUV, Coupe, etc.                 |
| `highway MPG`        | Highway mileage                         |
| `city mpg`           | City mileage                            |
| `Popularity`         | Popularity score                        |
| `MSRP`               | Manufacturer’s suggested retail price   |


## 🧹 Data Cleaning Steps

- Renamed columns for better clarity.
- Filled missing values using domain logic and statistical methods:
  - `Fuel Type`: Mode by make.
  - `Cylinders`: Median.
  - `Number of Doors`: Mode by make.
  - `Market Category`: Mode.
- Removed **715 duplicate rows**.
- Handled **outliers** in features like `Horse Power` and `highway MPG`.
- Converted column data types where necessary.


##  Key Questions Explored

###  Data Quality & Preparation
1. How many missing values were in the dataset, and how were they treated?
2. What strategy was used to fill missing values in `Fuel Type`, `Cylinders`, and `Number of Doors`?
3. How many duplicate records were found, and what impact did removing them have?
4. How were outliers in columns like `highway MPG` and `Horse Power` identified and treated?
5. What changes were made to improve column naming and data types?

###  Univariate & Bivariate Insights
6. Which car manufacturers dominate the dataset, and which are rare?
7. Which models are most and least common?
8. What are the top fuel types and their respective share?
9. How does city and highway mileage distribute across all cars?
10. How does `Transmission Type` affect vehicle pricing?
11. What is the average, minimum, and maximum MSRP of vehicles?
12. How have car prices changed over time?
13. Which vehicle sizes tend to be most expensive or most fuel-efficient?
14. What brands offer the best and worst mileage in city and highway driving?
15. Is there a strong correlation between `Horse Power` and `MSRP`?
16. Does the number of doors influence the vehicle's price?
17. What does the correlation heatmap reveal about relationships among numeric features?

###  Category & Segment Trends
18. Which vehicle styles (e.g., Sedan, SUV, Coupe) are most popular and/or expensive?
19. Are exotic or performance cars consistently outliers in horsepower or price?
20. How does the `Market Category` relate to price and vehicle type?


## Visualizations Used

- Bar plots (brands, models, MPG, MSRP)
- Pie charts (fuel types, transmission types)
- Box plots (outliers in MPG, horsepower, cylinders)
- Histograms & KDE plots (MPG distribution)
- Heatmaps (correlation matrix)
- Scatter plots (Horse Power vs MSRP)
- Line plots (Year vs MSRP)

## Summary of Insights

- **Chevrolet, Ford, and Toyota** dominate the dataset.
- **Bugatti, Maybach, Ferrari, and McLaren** are the most expensive brands.
- **Electric and premium fuel vehicles** tend to show better fuel efficiency.
- **Vehicle size** and **horsepower** are positively correlated with price.
- **Automatic transmissions** are more common and generally more expensive.
- A small number of outliers (like Bugatti's 1001 HP engine) have large impacts on overall statistics.
