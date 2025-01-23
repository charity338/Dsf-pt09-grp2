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
1. IMBD database - IMDB data source analysis
2. Box Office Mojo-BOM movie company analysis
3. Rotten Tomatoes-
4. TheMovieDB- 
5. TheNumbers-

*Description of data*
1. bom_movie_gross.csv - Our data has a total of 5 columns and 3387 rows. foreign_gross has 1350 missing values. domestic_gross has 28 missing values. studio has 5 missing values. foreign_gross (object) column needs to be converted to numeric.
2. tn_movie_budgets.csv -the dataset has 5782 rows and 6 columns.In the production_budget, domestic_gross and worldwide_gross columns,  remove currency sign and commas to make them fully numeric.combine both the domestic gross income and worldwide gross income into a new column called total gross income and this will form the basis of our analysis later.

*Data exploration*
.After reviewing the data, we perfomed exploratory data analysis(EDA) to identify trends and patterns that might influence movie success.
.Data was cleaned and prepared for analysis by handling missing values, renaming columns for clarity, and combining relevant datasets.

*visualizations*
1. bom_movie_gross.csv - 
 a) We first used  a bar chart that shows the top 10 movie studios ranked by their total domestic gross revenue (how much money the movies made in the United States).
 b) secondly we used a histogram that shows the distribution of the release years of the movies in the dataset, this will help us know which years the movies were released most.
 c) lastly, we used a correlation matrix heatmap, which is used to visualize the relationships between different numerical variables in the dataset. 

2. tn_movie_budgets.csv-
A scatter plot was used to visualize the relationship between production budget and total gross income.production budget on the x-axis and total gross income on the y-axis. If there's a positive relationship, you’ll likely see the points trending upwards from left to right. This would visually support the alternative hypothesis (Ha), where you expect that an increase in the production budget leads to an increase in the total gross income. 

## conclusion

1. bom_movie_gross.csv - 
Conclusion
Foreign gross earnings are generally higher than domestic gross, as indicated by the higher mean and median values. The foreign gross has greater variability compared to domestic gross (higher standard deviation i.e. $ 138.18 million.

2. tn_movie_budgets.csv
 In conclusion, the results of the linear regression analysis indicate a significant positive relationship between production budget and total gross income. The R-squared value of 0.547 means that approximately 54.7% of the variation in total gross income is explained by the production budget, which suggests a moderately strong fit of the model. The very low p-value (0.00) confirms that this relationship is statistically significant. Additionally, the coefficient of 4.2460 implies that for every 1-dollar increase in the production budget, total gross income increases by approximately 4.25 dollars on average. This supports the alternative hypothesis (Ha) that increasing the production budget leads to higher total gross income.














