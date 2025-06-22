# Netflix and the Problem Context:
We perform an Exploratory Data Analysis on the Netflix movie dataset to answer two business problems for the business, on content and growth.
1) Business Problem 1: Netflix, the streaming company wants to understand its existing content catalog. What are the dominant content types (Movie vs TV Show), and how are they distributed by year and genre?
2) Business Problem 2: Netflix wants to understand content diversity and which countries dominate which genres. Where are there gaps to expand?

# The Analysis Solution:
1) We obtain a dataset from Kaggle on Netflix Movies and TV Shows.
2) We explore the data to identify any issues and clean the data. As there were cells with multiple values, we normalize two columns relevant for the analysis. 
3) Then we conduct the analysis using data analysis techniques to solve the business problem.
4) We write insights from each step in the analysis and propose recommendations.

## Prerequisites:
1) Install packages, pandas, numpy, matplotlib, and seaborn.
2) For the world map, we install pycountry and plotly.express.
3) We recommend Jupyter Notebook if you wish to run the code, the file can be downloaded directly (Netflix_Analysis_EDA.ipynb).

## Input:
We use the netflix_titles_Nov2019.csv file from Kaggle as the basis for the analysis.
We form our own business case as mentioned in the problem context above.
We use Python for the analysis.

## Output: 
We produce several charts for analysis and draw insights.
Charts include: 
1) Dominant Content Types
2) Content Added to Netflix by Year
3) Top 10 Genres
4) Trends by Year
5) Top Content Producing Countries
6) Genre vs Country Heatmap
7) Number of Titles Per Country in a World Map

#### Insights are mentioned in each section in the analysis. 

## Suggestions for Netflix as a Business
- **Insight:** The United States dominates content production, followed by India and the UK.
- **Recommendation:** Invest in regional content production in emerging markets like Southeast Asia, Africa, Eastern Europe.
- **Insight:** From 2014 to 2019, content added yearly grew significantly—almost tripled by 2017.
- **Recommendation:** Maintain consistent but curated growth in content to ensure quality is not sacrificed for volume. To make a clear decision, it would be good to identify if there was a growth in revenue with content growth.
- **Insight:** Most popular genres are International Movies, Dramas, Comedies, and International TV Shows.
- **Recommendation:** Launch genre-based user journeys (e.g., curated playlists, interactive choices) to increase engagement and time spent on platform.
- **Insight:** Some countries and genres have minimal representation.
- **Recommendation:** Identify white-spaces in the genre-country matrix where Netflix has little presence and fill these gaps with short-form pilots or other content approaches.
