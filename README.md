Zomato Restaurant Performance Analysis

This project provides an end-to-end analysis of restaurant data from Zomato, focusing on key factors that drive restaurant performance, including ratings, cost, location, and service offerings.

The analysis is structured into three main components: data preprocessing, exploratory data analysis (EDA), and a final performance dashboard.

📂 Project Structure

File Name

Description

Data Preprocessing.ipynb

Handles the initial setup, database connection, data cleaning, and feature engineering necessary for the analysis.

Zamato EDA .ipynb

Contains the core Exploratory Data Analysis (EDA) with visualizations to uncover relationships between variables like cost, menu size, and rating.

DashBoard.pbix

The Power BI source file containing the interactive dashboard, data model, and all visualizations.

DashBoard.pdf

The final presentation document (likely exported from Power BI) showcasing key metrics and insights derived from the analysis in a static visual format.

🛠️ Prerequisites and Setup

This project relies on a connection to a MySQL database for both data loading and analysis.

Database: Ensure a MySQL instance is running with a database named minor_project.

Authentication: Update the connection parameters in both Jupyter notebooks (Data Preprocessing.ipynb and Zamato EDA .ipynb) to match your local setup:

username = "root"
password = "your_password"
host = "localhost"
database = "minor_project"



Libraries: The following Python libraries are required:

pandas

numpy

matplotlib

seaborn

sqlalchemy (specifically with mysql-connector)

Dashboard Software (New Requirement): To view or edit the interactive dashboard, Microsoft Power BI Desktop is required to open the DashBoard.pbix file.

📊 Key Findings and Insights

The analysis identified several factors strongly influencing restaurant performance and customer satisfaction:

1. Overall Performance Metrics

The analysis covers $\approx 8,700$ unique restaurants.

The Global Average Rating is $\approx 2.98$ (categorized into Poor, Average, Good, and Excellent).

The Average Cost for Two is $\approx 360$ (currency unit likely INR).

2. Impact of Service Offerings

The availability of certain services significantly impacts customer perception and ratings:

Restaurants that offer Online Ordering and Table Booking tend to have noticeably higher average ratings compared to those that do not, suggesting these features are highly valued by customers.

3. Geographical Analysis

Top Performing Locations: Neighborhoods such as Church Street, Brigade Road, Lavelle Road, and Residency Road show a high cumulative sum of ratings, indicating high activity and generally good performance.

Average Rating by Cuisine: Specific cuisine types are more highly rated than others, providing insights into market demands and culinary quality standards across different categories.

4. Menu Depth vs. Rating

Positive Correlation: The EDA shows a positive correlation between the number of dishes offered on a menu and the final restaurant rating.

Conclusion: While a larger, more diverse menu can contribute to higher customer ratings, the relationship is not perfectly linear. This suggests that other factors—such as food quality, ambiance, and service—are also critical determinants of the final rating.

🚀 How to Run the Project

Clone this repository (assuming this file is part of a repo).

Set up your MySQL database and ensure the connection details in the notebooks are correct.

Run Data Preprocessing.ipynb first: This notebook handles the necessary data cleaning and feature engineering (like categorizing costs and ratings) before analysis.

Run Zamato EDA .ipynb: Execute this notebook to reproduce the exploratory visualizations and generate analytical insights.

Review the Dashboard: Open DashBoard.pbix in Power BI Desktop for the interactive experience, or review DashBoard.pdf for the final report view.
