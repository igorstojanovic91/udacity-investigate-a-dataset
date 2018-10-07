# udacity-investigate-a-dataset

# Udacity Data Analyst Term 1 Project: Investigate a Dataset (TMDb movie data)

In this project, I analyzez a dataset and communicated my findings about it. I used the Python libraries NumPy, Pandas, and Matplotlib to do the analysis

This Python script is written for Project 3 (Term 1) of Udacity's Data Analyst Nanodegree (DAND) and is used to explore TMDb movie data. But what determines if a movie is considered as good or bad? There could be several factors influencig the quality of a movie, as for example the budget, genre, etc. This little project helped the author to improve his data analytics skills and explore some of the success criteria for movies.

First some Data Wrangling was applied, before the data was cleaned in order to perform Exploratory Data Analysis.

# How to run the script
You can run the script using a Python integrated development environment (IDE). This script is written in Python 3, so you will need the Python 3.x version of the installer. The code was written in Jupyter Notebook.


# Datasets
This data set contains information about 10,000 movies collected from The Movie Database (TMDb), including user ratings and revenue.

Certain columns, like ‘cast’ and ‘genres’, contain multiple values separated by pipe (|) characters.
The final two columns ending with “_adj” show the budget and revenue of the associated movie in terms of 2010 dollars, accounting for inflation over time.

Variables:
- id
- imdb_id
- popularity
- budget
- revenue
- original_title
- cast
- homepage
- director
- tagline	
- keywords
- overview
- runtime
- genres
- production_companies
- release_date
- vote_count
- vote_average
- release_year
- budget_adj
- revenue_adj

# Files
- tmdb-movies.csv

# Questions to answer
- Which genres are most popular from year to year?
- What kinds of properties are associated with movies that have high revenues?
- Did movies with higher vote count received a better rating?
- What were the most popular produced genres in 2000 compared to 2015?
- How did the amount of produced films changed over time?

# Findings
The first research question "Which genres are most popular from year to year?" has shown surprising results, as the most popular genre differed a lot. To the authors surprise, only in 11 occasions the most frequent produced genres was also voted as best genre by the users. In all remaining 40 occasions the two values differed.

The second research question "What kinds of properties are associated with movies that have high revenues?" shows interesting result. The numeric columns of "popularity, budget and vote_count" show the highest correlations. One can argue that movies with higher budgets are able to receive higher revenues, nevertheless, the correlation is not on a very high level. Vote_count is indicating that the more people vote for a movie, the higher the revenue is. Most probably, this is not a good indicator for high revenue movies. High revenue movies indicate that they are most commonly directed by Matt Damon, cast Tom Cruise as actor and contain the genre Action
.
The third research question "Did movies with higher vote count received a better rating?" does not indicate that movies with a higher vote_count receive a higher vote_average. Also by considering columns with more than 2000 vote_count does not change the impression. Furthermore, the corralation does not indicate that higher vote counts result in higher vote averages.
The forth research question "What were the most popular produced genres in 2000 compared to 2015?" indicate that in the year 2015 dramas were by far the most frequent produced movies, followed by thrillers and action. In 2000 the most frequent produced genre was thriller, followed by action and comedies. The bar chart indicates that in 2015 much more movies were produced compared to the year 2000.

The fifth research question "How did the amount of produced films changed over time?" reveals that the amount of produced films significantly increased from 1960 to 2015. Up to 1983 not more than 100 movies were prodcued per year, while in 2014 700 movies were produced. A strong increase in movie production can be obsorved between 1997-2009. One has to consider that the line chart does not show accurate results, as many rows from the original dataset were dropped.

All results are limited to the underlying data set and as no advaned statistics were performed, the results can only be treated as indicators and are not generalizable. Furthermore, one has to consider that many entries in the dataset have been removed due to missing data
