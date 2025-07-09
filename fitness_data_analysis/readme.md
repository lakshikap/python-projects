# Fitness Data and Problem Context

One of my customers wanted to understand useful insights on the fitness activities which were not available to him right away on the fitness watch app. He engages in a variety of fitness activities throughout the year, and wanted to know specifically:

1) A summary of the fitness activities and notable insights.
2) The average heart rate at which most number of calories are lost.
3) The most effective activity for losing calories, and  He also wanted to understand some useful insights on the 

## Why?

The current fitness watch data does not provide key insights, over a period. By visualizing trends over time, the analysis helped the customer discover high-impact workouts, optimize his exercise intensity, and personalize his fitness strategy. This empowered him to make data-driven decisions, improve time efficiency, and stay motivated through long-term progress tracking.

## The Approach and Solution

1. The customer shared the raw dataset from his fitness watch. This dataset had 37 columns including: Activity Type,	Date,	Favorite	Title,	Distance,	Calories,	Time,	Avg HR,	Max HR,	Aerobic TE,	Best Lap, Time,	Number of Laps,	Max Temp,	Moving Time,	Elapsed Time,	Min Elevation,	Max Elevation,	Time (seconds) etc.
2. Based on the problem context, I explored and reduced the data to retain 16 relevant columns. Thereafter I cleaned and applied transformations as needed. For example, I converted date to datetime format, and extracted time in minutes. 
3. Then I conduct the analysis using data analysis techniques to solve the customer problem. This analysis primarily uses pandas, matplotlib, and seaborn libraries.
4. I prepared a report on insights from each step in the analysis and propose recommendations. As a result, the customer provides a satisfied client testimonial.
<img width="644" alt="Screenshot 2025-07-09 at 2 20 30 PM" src="https://github.com/user-attachments/assets/8e2e1e42-8891-443b-bea6-90e14ba4f087" />

## Input:

I use the fitness watch dataset provided by the client. We do not share it publicly due to privacy concerns. 

## Output: Insights and Recommendations 

I created several charts for analysis, analyzed insights and made recommendations. 

1) Activity distribution over time.
<img width="317" alt="image" src="https://github.com/user-attachments/assets/798ce0bc-a449-429a-a86c-e82a4106f147" />



3) 

## Limitations:
1) The dataset for 5 years had only 700 rows and was too small for making accurate interpretations / recommendations for years with low data points.
2) There were a large number of rows with empty values.
3) There was a manually added 'Year' column at the end which was redundant for the analysis, as the real data was adequate.
