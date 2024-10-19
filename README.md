# TMDB-Movies-Data-Analysis

## Tools Used:
- Visual Studio Code
- Python
- Numpy
- Pandas

## Dataset Description

This dataset contains information about movies extracted from TMDB. The dataset contains movies from 1960 to 2015. Including user ratings and revenue. Original data from [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).

## Columns Descriptions
- `id`: A unique identifier for each movie entry.	
- `imdb_id`: The IMDb ID of the movie.
- `popularity`: A numeric measure of the movie's popularity.	
- `budget`: Movie's production budget in USD.	
- `revenue`:  Movie's total revenue in USD.	
- `original_title`:  The original title of the movie.
- `cast`:  A list of actors and actresses in the movie.
- `homepage`:   The official website of the movie.
- `director`: Name(s) of the director(s) of the movie (separated by "|" if there are more than one director).	
- `tagline`:  A short phrase or slogan that summarizes the movie's plot or theme.
- `keywords`: Key themes or topics  associated with the movie.
- `overview`: A brief summary or description of the movie's plot. 	
- `runtime`: Length of the movie in minutes.
- `genres`: Categories or types of movie genres of the movie separated by "|".
- `production_companies`: Companies involved in producing the movie.
- `release_date`:	Date when the movie was released.
- `vote_count`: Number of votes or ratings the movie has received.	
- `vote_average`: Average rating of the movie	
- `release_year`:	Year the movie was released.
- `budget_adj`: Adjusted budget (possibly for inflation).
- `revenue_adj`: Adjusted revenue (possibly for inflation).

## Questions For Analysis:
- Do movies with high popularity achive high revenue?
- What are the most filmed genres in the whole dataset?
- Is there a correlation between a movie budget and its revenue?

## Data Wrangling:

Data can be found in `movies.csv` file in this repository. The data is originally from [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).

## Data Cleaning:

We dive deeper into exploring our dataser and perform cleaning operations like(dropping columns, handling NaNs and converting datatypes). All of this will help us to reach more accurate result in answering questions.

- Our dataset consists of a total of 10866 rows and 21 columns.
- We have only 1 duplicated row which would be droped.
- Some columns wont be useful in answering our questions using analysis.
- Few columns have many missing values that needs to be handled.
- Columns `cast` `director` `genre` have values saperated with a '|'.
- `release_date`'s data type needs to be casted.
- We can append a column for the movie `profit` using formula.
- `vote_average` better be presented as a catecorical variable that groubs multible ratings values.
- We may also catigorize `profit` column for better EDA

## Exploratory Data Analysis:

After cleaning our dataset it consists of 10840 records with 10 columns, it does not have any dupicates or null values, and the datatypes are consistant with suitable categorical variable to address our questions.Then we performed some analytics and created some visulization to answer our questions.

**Q1: Do movies with high popularity achive high revenvue?**

More popuar movies recieve way more revenue than the less popular movies.

**Q2: What are the most filmed genres in this whole dataset?**

- `Drama`, `Comedy` and `Action` are the top three filmed genre movies in our dataset.
- `Drama` genre contributes 22.6% of all the genres in the dataset.

**Q3: Is there a correlation between a movie budget and its revenue?**

There is a positive correlation between `budget` and `revenue` indicating a relation between them with little outliers.

