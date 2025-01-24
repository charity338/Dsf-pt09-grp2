# GROUP TWO PHASE TWO DATA SCIENCE PROJECT 
## group memebers;
1. Humphrey Matagaro
2. Charity Nguru
3. Jael Kirwa
4. Evelyn Mwangi
5. Okech Maximillan
6. Samuel Maina

# # Project Overview
This project explores current movie trends to help guide the business desicions of a newly launched movie studio.Our project goal is to analyze various data sets from reputable movie sources such as Box Office Mojo(BOM), IMDB, Rotten tomatoes and The Numbers , to identify actionable insights that the movie studio can use to produce films with hih box-office potential.

## Business understanding
*Stakeholder;* 
The head of the new movie studio.
*Business Problem;*
The new company wants to understand the factors that influnce box-office perfomance and how they can apply this knowledge to create films that resonate with audiences and make profit.

*key business questions*
Which are the best performing movies categories to produce?
Which demographics watch movies ?
What each demographic prefer to watch ?

## Data understanding and Analysis
*source of data*
The analysis is based on five datasets from various movie industry sources;
1. IMBD database - 
2. Box Office Mojo-
3. Rotten Tomatoes-
4. TheMovieDB- 
5. TheNumbers-

*Description of data*
1. bom_movie_gross.csv - Our data has a total of 5 columns and 3387 rows. foreign_gross has 1350 missing values. domestic_gross has 28 missing values. studio has 5 missing values. foreign_gross (object) column needs to be converted to numeric.
2. tn_movie_budgets.csv -the dataset has 5782 rows and 6 columns.In the production_budget, domestic_gross and worldwide_gross columns, we remove currency sign and commas to make them fully numeric.Then combine both the domestic gross income and worldwide gross income into a new column called total gross income and this will form the basis of our analysis later.
3. im.db - This data contains information about movies, including their unique identifiers, average user ratings, and the number of votes cast by viewers.
4. tmdb_movies.csv - This dataset has 26,517 rows and 10 coloumns.This data includes popular and well-known movies across different genres and release years.


*Data exploration*
.After reviewing the data, we perfomed exploratory data analysis(EDA) to identify trends and patterns that might influence movie success.
.Data was cleaned and prepared for analysis by handling missing values, renaming columns for clarity, and combining relevant datasets as well as hypothesis for various business questions.

*visualizations*
1. bom_movie_gross.csv - 
 a)  a bar chart was used to show the top 10 movie studios ranked by their total domestic gross revenue (how much money the movies made in the United States).
 b) secondly we used a histogram that shows the distribution of the release years of the movies in the dataset, this will help us know which years the movies were released most.
 c) lastly,  a correlation matrix heatmap was used, to visualize the relationships between different numerical variables in the dataset. 

2. tn_movie_budgets.csv-
A scatter plot was used to visualize the relationship between production budget and total gross income.production budget on the x-axis and total gross income on the y-axis. If there's a positive relationship, you’ll likely see the points trending upwards from left to right. This would visually support the alternative hypothesis (Ha), where you expect that an increase in the production budget leads to an increase in the total gross income. 

3.im.db (1)- 
 a) A histogram was used to visualize the distribution of movie runtimes (in minutes) and summarizes the descriptive statistics of the runtime_minutes column. From the visualization we have a movie with a minimum of 3 minutes and a long movie with 51420 minutes. These outliers heavily affect the mean. The median, however, is least affected by the outliers.
 b) A bar chart was used to visualize the distribution of movie genres based on their counts in the dataset.
 c) A barplot was used to filter and visualize genres whose percentages fall between 1% and 20% in the dataset, where ,(<1%) excludes very rare genres and (>20%) very common genres to focus on mid-range categories.Drama was the most popular.
 d) A box plot to visualize the distribution of quality_score across different quality_category levels in the im_ratings dataset, As quality category increases (from Low to High), the median and overall quality score also increase.The Medium category has the widest distribution, while the High category shows the least spread in scores.
 e) A grid of histograms for the quality_score distribution across the Low, Medium, and High categories. Each histogram shows the frequency of scores within that specific category.
 f) A bar chart that shows the frequency of running minutes grouped into predefined ranges (e.g., "0-10 minutes," "10-20 minutes," etc.), and identifies the most common range.
 
 4. im.db (2)-
 a) A histoplot to show data distribution.
 b) A heatmap for plotting missing values.lots of missing values in runtime_minutes
 c) A heatmap to analyzes and visualizes the correlations between the numeric columns runtime_minutes, averagerating, and numvotes 
 d) A barplot to analyzes and visualizes the popularity of movie genres based on their frequency in the dataset,
In the film production industry as analysed in the data , The top 3 genres include;

            1. Drama
            2. Documentary
            3. Comedy
 e) Two scatter plot to visualize the correlation coefficient between average rating and number of votes and avg rating vs Runtime.low correlation is consistent  in both cases, indicating that neither number of votes nor runtime strongly predict rating. This therefore means that audience preference for movie runtime is subjective and does not impact movies rating.
 
 5.tmdb_movies.csv - 
 a) A histogram to visualize the distribution of movie popularity.The data is heavily right-skewed, meaning that the majority of movies have very low popularity scores, while a small number of movies are significantly more popular.The frequency of movies decreases sharply as the popularity score increases.
 b) A scatterplot was used to explore the relationship between "vote average" and "popolarity".Movies with higher popularity tend to have better ratings.
 c) A bar graph of movies by original language to provide insights into the dominance of English-language movies in the dataset.
 d) A bargrapgh on 15 most popular movies with their movie titles.
 e) A heatmap on the correlation between popularity, vote average and vote count.
 
 
## conclusion

1. bom_movie_gross.csv - 
Conclusion
Foreign gross earnings are generally higher than domestic gross, as indicated by the higher mean and median values. The foreign gross has greater variability compared to domestic gross (higher standard deviation i.e. $ 138.18 million.

2. tn_movie_budgets.csv
 In conclusion, the results of the linear regression analysis indicate a significant positive relationship between production budget and total gross income. The R-squared value of 0.547 means that approximately 54.7% of the variation in total gross income is explained by the production budget, which suggests a moderately strong fit of the model. The very low p-value (0.00) confirms that this relationship is statistically significant. Additionally, the coefficient of 4.2460 implies that for every 1-dollar increase in the production budget, total gross income increases by approximately 4.25 dollars on average. This supports the alternative hypothesis (Ha) that increasing the production budget leads to higher total gross income.
 
3.im.db (1)
From the analysis the DRAMA genre is the safest genre to produce based on the industry frequency of producing that genre. However, ACTIN-CRIME-DRAMA, despite having a small audience had the best quality score compared to the top 30 genres. This genre most-likely attracts enthusiats and mite skew the ratings in favor of the production company. The industry go-to runtime mintes ranged between 91-120 minutes with longer movies having fewer audiences. Therefore, for a Blockbuster movie with a big budget, the action-crime-drama genre is most likely going to have better reviews and a bigger impact on the audience. For medium to low budget, however, the drama genre seems most appropriate due to its safe numbers.

4. im.db (2)
The analysis indicates that there is no single dominant genre claiming the top spot, but there is strong evidence of market demand across multiple genres, particularly Drama, Action, Documentaries, Mystery, Sci-Fi, Crime, Thriller, War, Action, and Comedy. This suggests a diverse and wide-ranging audience base.

5. tmdb_movies.csv- 

High budget: Movies with high budgets OFTEN achieve greater popularity due to vast and intense marketing.
-Genre popularity: Certain genres like action, adventure, and fantasy rank high in popularity.
-Star power: Movies with renowned and famous actors and directors tend to attract larger audiences. 
-Release date: Factors like seasonality , holiday releases, and competition from others can impact popularity.
-Relationship with vote count: Higher vote counts generally indicate a larger audience base. -Impact of technological advancements: The use of advanced technology eg.streaming platforms have impacted movie production and audience engagement.








