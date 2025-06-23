# Netflix and the Problem Context:
I perform an Exploratory Data Analysis on the Netflix movie dataset to answer two business problems for the business, on content and growth.
1) Business Problem 1: Netflix, the streaming company wants to understand its existing content catalog. What are the dominant content types (Movie vs TV Show), and how are they distributed by year and genre?
2) Business Problem 2: Netflix wants to understand content diversity and which countries dominate which genres. Where are there gaps to expand?

## The Approach and Solution:
1) I obtain a dataset from Kaggle on Netflix Movies and TV Shows.
2) I explore the data to identify any issues and clean the data. As there were cells with multiple values, I normalize two columns relevant for the analysis. 
3) Then I conduct the analysis using data analysis techniques to solve the business problem. This analysis primarily uses pandas, numpy, matplotlib, plotly and seaborn.
4) I write insights from each step in the analysis and propose recommendations.

## Input:
I use the netflix_titles_Nov2019.csv file from Kaggle as the basis for the data analysis.
I form my own business case as mentioned in the problem context above.
I use Python for the data analysis.

## Output: 
I produce several charts for analysis and draw insights. Charts include: 
1) Dominant Content Types
<img width="556" alt="Screenshot 2025-06-23 at 7 44 47 PM" src="https://github.com/user-attachments/assets/e18ed483-d29a-4f4d-9a2d-8276b932fc6c" />
***Insights: Overall, Netflix has more Movies than TV Shows. The number of Movies is a little more than twice the number of TV Shows.***

3) Content Added to Netflix by Year
   <img width="864" alt="Screenshot 2025-06-23 at 7 44 54 PM" src="https://github.com/user-attachments/assets/63ccee21-17ed-4378-a797-844ff92a6feb" />

***Insights: There is a significant growing trend in content from 2015 to 2019. From 2014 to 2016 the number almost quadrupled each year. Then from 2016 to 2017 the content grew by 2.5 times.***
   
5) Top 10 Genres
<img width="872" alt="Screenshot 2025-06-23 at 7 45 02 PM" src="https://github.com/user-attachments/assets/dbd12771-c6ee-4eea-96e7-efd0e062d3f7" />

***Insights: The most common genres are International Movies and Dramas. Comedies and International TV shows were in close numbers at third place.***
  
6) Trends by Year
<img width="858" alt="Screenshot 2025-06-23 at 7 45 11 PM" src="https://github.com/user-attachments/assets/addb4d49-3748-4045-9670-1faa85f8f97c" />

***Insights: Movies and TV Shows grew significantly from 2014 to 2019. From 2014 to 2017, the numbers almost tripled. While the number od TV Shows were lesser than Movies, both segments grew significantly until 2019.***

7) Top Content Producing Countries
<img width="864" alt="Screenshot 2025-06-23 at 7 45 17 PM" src="https://github.com/user-attachments/assets/9e3c9aa5-d823-47c2-9614-2c41b64de424" />

***Insights: United States dominates content production on Netflix, while India comes in second and the United Kingdom as the third.***

8) Genre vs Country Heatmap
  <img width="869" alt="Screenshot 2025-06-23 at 7 45 26 PM" src="https://github.com/user-attachments/assets/1f080f66-666e-4e9b-b29c-9ae83f7fb221" />

***Insights: We see which countries dominate certain genres. United States dominates the Dramas, Comedies and Documentaries, while India leads in International Movies and Dramas.***

9) Number of Titles Per Country in a World Map
<img width="768" alt="Screenshot 2025-06-23 at 7 48 23 PM" src="https://github.com/user-attachments/assets/b839b757-d38e-45e8-bfb4-9fa2ebdf39f3" />

***Insights: The map allows you to hover over to identify content distribution by country. The USA domainates total content, and India comes in second.***

#### Insights are mentioned in each section in the analysis. 

## Suggestions for Netflix as a Business: Where are there gaps to expand?
1) **Insight:** The United States dominates content production, followed by India and the UK.
- **Recommendation:** Invest in regional content production in emerging markets like Southeast Asia, Africa, Eastern Europe.
2) **Insight:** From 2014 to 2019, content added yearly grew significantly—almost tripled by 2017.
- **Recommendation:** Maintain consistent but curated growth in content to ensure quality is not sacrificed for volume. To make a clear decision, it would be good to identify if there was a growth in revenue with content growth.
3) **Insight:** Most popular genres are International Movies, Dramas, Comedies, and International TV Shows.
- **Recommendation:** Launch genre-based user journeys (e.g., curated playlists, interactive choices) to increase engagement and time spent on platform.
4) **Insight:** Some countries and genres have minimal representation.
- **Recommendation:** Identify white-spaces in the genre-country matrix where Netflix has little presence and fill these gaps with short-form pilots or other content approaches.
