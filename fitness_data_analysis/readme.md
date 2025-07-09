# Fitness Data and Problem Context

One of my customers wanted to obtain more insights from the data tracked by his fitness watch. 
He engages in a variety of fitness activities throughout the year, and wanted to know the most effective activities for losing calories, and the heart rate which loses the most number of calories. He also wanted to understand some useful insights on the fitness activities which were not available to him right away on the watch. 

## Why?

The current fitness watch data does not provide key insights, over a period. By visualizing trends over time, the analysis helped him discover high-impact workouts, optimize his exercise intensity, and personalize his fitness strategy. This empowered him to make data-driven decisions, improve time efficiency, and stay motivated through long-term progress tracking.

## The Approach and Solution

1. He shared the raw dataset from his fitness watch. This dataset had 37 columns including: Activity Type,	Date,	Favorite	Title,	Distance,	Calories,	Time,	Avg HR,	Max HR,	Aerobic TE,	Best Lap, Time,	Number of Laps,	Max Temp,	Moving Time,	Elapsed Time,	Min Elevation,	Max Elevation,	Time (seconds) etc.
2. Based on the problem context, I explored and reduced the data to retain 16 relevant columns. Thereafter I cleaned and applied transformations as needed. For example, I converted date to datetime format, and extracted time in minutes. 
3. Then I conduct the analysis using data analysis techniques to solve the customer problem. This analysis primarily uses pandas, numpy, matplotlib, plotly, seaborn and pycountry libraries.
4. I prepared a report on insights from each step in the analysis and propose recommendations. As a result, the customer provides a satisfied client testimonial.
<img width="644" alt="Screenshot 2025-07-09 at 2 20 30 PM" src="https://github.com/user-attachments/assets/8e2e1e42-8891-443b-bea6-90e14ba4f087" />


