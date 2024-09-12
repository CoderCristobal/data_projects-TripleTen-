Zuber Ride-Share Analysis: Impact of External Factors and Passenger Preferences
Project Overview
This project focuses on analyzing ride-sharing patterns for Zuber, a new company launching in Chicago. The primary goal is to understand passenger preferences and assess the impact of external factors, such as weather conditions, on ride frequency and duration. Using available data from competitors, a hypothesis is tested regarding the effect of weather on rides between the Loop and O'Hare International Airport.

Project Breakdown
Step 1: Data Parsing and Weather Information Retrieval
The first step involves writing code to extract weather data from Chicago in November 2017, using a web scraping technique to access the following data. This data will be used to determine weather conditions that may impact ride durations and demand.

Step 2: Exploratory Data Analysis (SQL)
We analyzed competitor data by performing SQL queries on Zuber’s dataset to understand the demand for different taxi companies:

Taxi Ride Volume: We calculated the number of taxi rides for each company on November 15-16, 2017, sorting them by ride count.
Top Taxi Companies: We focused on companies containing "Yellow" or "Blue" in their names during November 1-7, 2017.
Leading Taxi Companies: The most popular taxi companies, Flash Cab and Taxi Affiliation Services, were compared with other companies, grouping lesser-known competitors as "Other" to study market dynamics.
Step 3: Testing Hypotheses on Weather Impact
We tested the hypothesis that the duration of rides between the Loop and O'Hare Airport changes on rainy Saturdays. By retrieving weather conditions from a dedicated dataset and analyzing ride durations during rainy and non-rainy periods, we categorized rides based on the presence of "rain" or "storm" and tested for statistically significant differences.

Step 4: Data Visualization (Python)
We extended the analysis using two additional datasets:

project_sql_result_01.csv: Number of rides by taxi companies on November 15-16, 2017.
project_sql_result_04.csv: Average number of rides that ended in different Chicago neighborhoods in November 2017.
For each dataset, we:

Imported and cleaned the data, ensuring correct data types.
Identified the top 10 neighborhoods with the highest number of drop-offs.
Created visualizations to showcase the number of rides per company and the most popular neighborhoods for drop-offs.
Step 5: Hypothesis Testing (Python)
We conducted hypothesis testing using data from project_sql_result_07.csv, which contains the duration of rides from the Loop to O'Hare International Airport. The goal was to test if weather conditions affected ride duration on rainy Saturdays, using a significance level of 0.05.

Results
Taxi Ride Analysis: Flash Cab led with 19,558 trips, followed by Taxi Affiliation Services with 11,422 trips. Companies like Yellow Cab and Medallion Leasing also had a strong market presence. Flash Cab’s dominant position suggests it has a well-established service, but the taxi industry in Chicago remains competitive.

Neighborhood Drop-Offs: The Loop was the most frequent drop-off location, followed by River North and Streeterville. Sheffield & DePaul had the lowest average number of trips, indicating differences in demand across neighborhoods.

Hypothesis Test Conclusion: The null hypothesis that "the average duration of rides from the Loop to O'Hare International Airport does not differ on rainy Saturdays" was rejected with a very low p-value, indicating that weather significantly impacts ride duration. Rainy Saturdays caused longer ride times due to likely delays.

Conclusion and Recommendations
Based on the analysis:

Taxi Industry Insights: Flash Cab and Taxi Affiliation Services lead the Chicago market. Zuber could focus on competing with these services by enhancing efficiency and fleet management.
Weather Impact: Weather conditions, especially rain, significantly affect ride durations. Zuber can use this insight to optimize pricing strategies, implement surge pricing during bad weather, and prepare for longer travel times to maintain customer satisfaction.
Suggestions for Further Improvements
Customer Segmentation: Explore segmentation to offer personalized promotions based on usage patterns, weather, and neighborhood preferences.
Dynamic Pricing: Implement a dynamic pricing model that adjusts fares based on weather conditions, time of day, and location to increase revenue and manage demand.
Service Expansion: Investigate under-served areas like Sheffield & DePaul, potentially targeting them with special offers or increased availability.
By focusing on passenger preferences and leveraging external factors like weather, Zuber can better understand market dynamics, enhance operational efficiency, and improve customer satisfaction.
