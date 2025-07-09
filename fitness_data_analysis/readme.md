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

I use the fitness watch dataset provided by the client. I did not share it publicly due to privacy concerns. 

## Output: Insights and Recommendations 

I created several charts for analysis, analyzed insights and made recommendations. Here is the report I provided for the customer. 

1) Fitness activity distribution over time.

<img width="317" alt="image" src="https://github.com/user-attachments/assets/798ce0bc-a449-429a-a86c-e82a4106f147" />

**Insight:** Your plot of activity entries per year shows noticeable variation over the years. Noticeably, 2020 and 2021 had significantly higher activity logging.

**Recommendation:** Identify what led to increased consistency during peak years (e.g., structured plan, goal setting). Use that pattern to replicate consistent activity this year.
![image](https://github.com/user-attachments/assets/ae98c695-cd65-4550-b8ac-83c57f2ae543)

2) Most common activities

<img width="338" alt="image" src="https://github.com/user-attachments/assets/696107a5-ded2-4da2-9979-31b96f6ac059" />

**Insight:** Strength training, treadmill running, walking and running dominate your workout history. 

**Recommendation:** You can introduce more balanced cross-training workouts to reduce repetitive strain and cardiovascular fitness diversity.

3) Activity count and type by year

<img width="375" alt="image" src="https://github.com/user-attachments/assets/8f4add0e-dca6-40da-9b9a-c30226cfd74d" />

**Insight:** Some activity types are more seasonal across years. However, there is no consistent pattern or workout type in this aspect, except a low but recurring walking activity recorded over the years 2020 to 2024 with some appearance in 2025.

**Recommendation:** Consider seasonal workout planning to maintain motivation. Walking might be your easiest and favourite workout, hence focus on improving the same as much as possible.

4) Correlation analysis by activity type (Relationship between distance, calories, average heart rate and time)

I created heatmaps to identify the relationship among distance, calories, average heart rate and time in minutes, per activity. Your heatmaps revealed unique relationships per activity. Let's explore these relationships in detail in the next section.

   i) Treadmill running
   
<img width="224" alt="image" src="https://github.com/user-attachments/assets/fec682bd-6fb0-4e3e-a9f7-00a2a4160e0c" />

**Insight:** There is a moderate positive relationship among distance with calories, time and average heart rate. This means that treadmill running burns calories to some extent. The more time you spend on a treadmill means, moderate calories burned. Also, average heart rate slightly lets you burn moderate level of calories. 

**Recommendation:** Treadmill workouts are effective for controlled cardio, increase time and pace gradually for aerobic development and endurance.

  ii) Walking 

<img width="249" alt="image" src="https://github.com/user-attachments/assets/03a9899a-d021-448d-9728-e7aa0a0ca95b" />

**Insight:** There is a strong positive relationship between calories and distance. That means the more you walk the more you burn calories and get in shape. While a moderately increased heart rate may burn calories, a higher or increasing heart rate does not always mean high calorie burn. 

**Recommendation:** Encourage longer walks at brisk pace for consistent calorie burn. 

  iii) Multisport
Not enough data to suggest a recommendation. Consider logging more detailed sessions or separating sports by type for better / useful insights. ![image](https://github.com/user-attachments/assets/db0e5d37-fc35-4a7a-8063-ee4ab942e480)

  iv) Strength Training

<img width="266" alt="image" src="https://github.com/user-attachments/assets/75c0e458-22c8-4f7f-97ce-f227c9172de2" />

**Insight:** There is a strong positive relationship between time spent and calories burned and time spent. That means the more your strength train, the more you sweat and burn calories. Average heart rate is lower, with moderate correlation to calories. A higher or increasing heart rate generally leads to more calories burned.

**Recommendation:** Increasing workout duration is an efficient way to increase calorie burn. You can also raise heart rate using intensity techniques in strength training.

  v) Running

  <img width="242" alt="image" src="https://github.com/user-attachments/assets/15ce080c-e9eb-4174-8a71-33726bd28c63" />

**Insight:** There is a strong positive relationship of distance with calorie burn rate and average heart rate increase. That means the more you run on natural terrain, the more you burn calories.

**Recommendation:** Aim to increase distance gradually each week to improve endurance and calorie burn. Alternate low-average heart rate long runs with high-average heart rate short runs for balance. E.g., A 30-minute high heart rate run may burn more than a 60-minute slow jog.

  vi) Pool Swim

<img width="239" alt="image" src="https://github.com/user-attachments/assets/70db405c-3260-42ac-b617-622d7dbd6ed9" />

**Insight:** There is a strong positive relationship between distance with calories burned and average heart rate. That means the more you swim the more you burn calories. Average heart rate has moderate positive correlation to calories burned and distance.

**Recommendation:** Focus on building endurance through higher distance (laps) and improving pace.

**Note:** There is a negative correlation of time with distance and calories, which is abnormal. Be aware of how time is being tracked, ensure it records active swim and not total pool time. 

5) Time vs Calories Burned

  1) Overall time vs calories burned
<img width="318" alt="image" src="https://github.com/user-attachments/assets/15b8fdfc-66c2-44f2-92dd-63da52a3df31" />

**Insight:** Overall, on all activities, spending more time on a workout means more calories are burned. However, I have to isolate the activities to identify their relationships separately.

  i) Treadmill Running

<img width="312" alt="image" src="https://github.com/user-attachments/assets/a5550345-b90d-4bf4-821c-b2a860e97f7c" />

**Insight:** For treadmill running, the maximum calories were burned at average heart rate of 158. However, it is important to note that, calories are burned both gradually over time and dynamically based on heart rate. 

**Recommendation:** A heart rate of 160+ bpm during walking (as in the red point) is unusual and may not be safe for everyone. Aim for moderate-higher heart rate zones (130–150 bpm) during walks to increase calorie expenditure.
Refer to this link for a guideline for your age range: 
https://www.hopkinsmedicine.org/health/wellness-and-prevention/understanding-your-target-heart-rate#:~:text=The%20maximum%20rate%20is%20based,or%2085%20beats%20per%20minute

  ii) Walking 

<img width="319" alt="image" src="https://github.com/user-attachments/assets/a696697c-9577-4525-8ed0-3b8018730e38" />

**Insight:** For walking, the maximum calories were burned at average heart rate of 161. However, it is important to note that, calories are burned both gradually over time and dynamically based on heart rate.

**Recommendation:** Don’t chase maximum heart rate every time. The red dot (heart rate 158, Cal 673) may not be sustainable for your age or ideal for daily sessions. 
Refer to the above link for a guideline for your age range.

  iii) Strength Training

<img width="309" alt="image" src="https://github.com/user-attachments/assets/6e3a1565-251d-4b74-be2b-77a53dc26190" />

**Insight:** For strength training, the maximum calories (959) were burned at average heart rate of 132. 

**Recommendation:** This is in the safe range, so strength training is safer for maximum calorie burn at a relatively low-average heart rate. High calorie burn doesn’t require the highest heart rate, but sustained intensity over time.

  iv) Running

<img width="312" alt="image" src="https://github.com/user-attachments/assets/2b5843cf-a44a-4e34-ba54-890c609584f2" />

**Insight:** For running, the maximum calories were burned at average heart rate of 173. The red dot (heart rate 173, Cal 800) may not be sustainable or ideal for daily sessions.
This suggests that running intensity (heart rate) is a strong predictor of calories burned.

**Recommendation:** Average heart rate of 170+ is near max for most adults. This requires solid recovery and should not be a daily target.
Target heart rates at 130-160 bpm for sustained calorie burn and endurance benefits. These points in that range show consistent calorie burn increases with rising heart rate. This is efficient aerobic training. 
Refer to this guide to understand more - https://www.mayoclinic.org/healthy-lifestyle/fitness/in-depth/exercise-intensity/art-20046887 

  v) Swimming

<img width="328" alt="image" src="https://github.com/user-attachments/assets/f5d685c8-29a6-4dce-a84b-0e0f8a406ec6" />

**Insight:** For pool swimming, at 167 heart rate, 91 calories were burned which is not an effective rate. The events recorded are likely short duration swims or inconsistent data.

**Recommendation:** Average heart rate isn’t the only driver of calorie burn in swimming. Unlike running, where heart rate and calorie burn align closely, swimming adds complexity.

6) Highest Calorie Efficiency

<img width="382" alt="image" src="https://github.com/user-attachments/assets/fa3f995c-8e10-4fa4-9c63-05f7c3c91d89" />

**Insight:** Overall, treadmill running delivers the highest calorie efficiency, burning approximately 536 calories per kilometer. This suggests that even short runs of high-intensity treadmill workouts can yield substantial energy expenditure, making it ideal for time-constrained workouts focused on fat loss.

**Recommendation:** Intriduce more treadmill running in your workouts. As you travel often, this is the best recommended workout for your routine, with the maximum calorie  burn rate against time and distance.

## Limitations:
1) The dataset for 5 years had only 700 rows and was too small for making accurate interpretations / recommendations for some activities/ years with fewer data points.
2) There were a large number of rows with empty values.
3) There was a manually added 'Year' column at the end which was redundant for the analysis, as the real data was adequate.
