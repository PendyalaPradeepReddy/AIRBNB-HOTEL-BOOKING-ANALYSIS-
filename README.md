🏡 Airbnb Hotel Booking Analysis: New York City Lodging Market Insights
Project Overview
This project provides a comprehensive data analysis of the New York City Airbnb lodging market. Utilizing a large, publicly available dataset, the study employs rigorous data cleaning, exploratory data analysis (EDA), and visualization techniques to uncover key trends and factors influencing listing availability, pricing strategies, and customer satisfaction.

The goal is to move beyond raw data and extract meaningful, actionable insights for hosts, guests, and industry enthusiasts navigating this dynamic urban accommodation landscape.

Problem Statement
The short-term lodging sector has been revolutionized by platforms like Airbnb. To better understand the mechanics of this market in a dense, high-demand city like New York, this analysis seeks to answer critical questions about listing dynamics. By discerning the relationship between various features—such as neighborhood, room type, price, and host identity—we aim to illuminate the operational and financial factors driving success in the NYC Airbnb ecosystem.

Key Questions Explored
The analysis focused on answering the following core business questions:

Property Distribution: What are the most common property and room types available in the dataset?

Geographic Trends: Which neighborhood groups have the highest concentration of listings and the highest average prices?

Pricing Factors: Is there a relationship between the construction year of a property and its average price?

Fee Structure: Is there a correlation between a listing's price and its mandatory service fee?

Host Performance: Are hosts with verified identities more likely to achieve higher average review rates?

Top Hosts: Who are the top 10 hosts based on their calculated host listing count?

Availability: Is there a correlation between the number of listings a host manages and the overall availability of their properties throughout the year?

Methodology and Findings
1. Data Preparation
Source: NYC Airbnb Open Data.

Cleaning Steps:

Handled and dropped 541 duplicate records.

Addressed missing values by dropping columns with low completeness (e.g., license, house_rules) or records with critical missing information (e.g., price, host identity).

Corrected data types (e.g., converting 'host id' to string, 'Construction year' to integer, and date fields).

Data correction was performed, notably fixing a misspelling of the 'Brooklyn' neighborhood group.

Outliers were addressed by dropping listings with unusual values, such as extremely high availability 365 days (> 500).

2. Key Analytical Results
Area of Analysis

Finding

Insight

Property Mix

The dataset is dominated by Entire home/apt and Private room listings.

The market primarily caters to renters seeking full privacy or budget-conscious private room options.

Pricing & Location

Manhattan has the highest average listing price (approx. $628), followed closely by Brooklyn (approx. $624).

Despite having a similar listing volume to Manhattan, Brooklyn commands prices almost as high, indicating strong demand.

Price vs. Service Fee

There is an extremely strong positive correlation (0.99999) between the price and the service fee.

The service fee is calculated as a near-fixed, direct percentage of the total listing price.

Host Verification

Verified hosts receive a marginally higher average review rate (3.28) than unconfirmed hosts (3.27).

Host verification has a minimal direct impact on review scores; other factors (e.g., service quality) are more dominant.

Room Type Reviews

Hotel rooms and Shared rooms generally receive the highest average review rates across all boroughs.

This suggests that while hotel rooms meet clear professional standards, the small pool of available shared rooms may benefit from hosts with exceptional customer service.

Listing Count vs. Availability

The correlation between a host's total listing count and their property availability is very weak (0.136).

Managing more properties does not make a host significantly more or less likely to keep their listings available throughout the year.

Technology Used
Language: Python

Core Libraries:

pandas: Data structuring, manipulation, and cleaning.

numpy: Numerical and array operations.

Visualization Libraries:

matplotlib.pyplot: Foundational plotting library.

seaborn: Advanced statistical visualization for complex data relationships.

plotly.express (Imported for use).

Next Steps
Potential future analysis directions include:

Time-Series Analysis: Analyzing the trend of price and review changes over time using the last review and Construction year data to identify market maturation.

Natural Language Processing (NLP): Analyzing the content of the house_rules and NAME fields to extract linguistic features that correlate with price or review scores.

Predictive Modeling: Developing a machine learning model to predict the price or review rate of a new listing based on its characteristics.
