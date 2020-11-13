# project-portfolio
Data Analysis projects


TMDb is an initialism that is almost similar to its more bigger counterpart: IMDb. Both are massive indexes for movie and television information, but The Movie Database differs from the Internet Movie Database in one key aspect that is TMDb is completely powered by its community.

The Movie Database is an online crowdsourced database for movie and television information. The metadata on movies and TV shows is contributed by the 1.1 million strong community. As of writing this, the site has indexed 393,000+ movies and 73,000+ TV shows across 39 languages.

This dataset is a collection of data on around 10000 movies.The primary goal of this is to perform detailed analysis and visualization to derive answers for the questions brainstromed.

We use numpy and pandas for Analysis, matplotib and seaborn for Visualization.

## Outline for Analysis

- Assessed the data and brainstormed questions that could be answered using the data
- Performed necessary cleaning steps to unify formats, deal with missing data and prepare the dataset for analysis
- Wrangled and explored the data using Pandas and Numpy to gather insights about the relationship between different aspects, created visualizations using matplotlib and made inferences to answer research questions

## Questions

Based on the the given attributes the following questions can be asked and answered:

- what are  genres available
- what is the most succesfull genre with respect to movies
- which star cast has most movies
- what are the movies with highest and lowest profits
- what are the movies with highest runtime
- Average revenue
- what are the movies with highest and lowest budgets

Obsevations from the data set:

- No unit of currency is mentioned in the dataset. For this analysis we will consider it as dollar as it is the most used international currency.

- vote_count is different for all the movies, so we cannot directly conclude the popularity of the movies based on the average vote count

Below are the tasks performed to clean the dataset:

- We need to remove unused column such as id, imdb_id, vote_count, production_company, keywords, homepage etc.
- Removing the duplicate rows (if any).
- Some movies in the database have zero budget or zero revenue, that means the value has not been recorded so we will be discarding such entries
- Changing release date column into date format.
- Replacing zero with NAN in runtime column.
- Changing format of budget and revenue column.

## Conclusions

Being a movie buff myself it was great working on this data set .We derived some intresting conclusions after the analysis.

Most commonly successfull movies have below characteristics.

- Average Budget must be around 63 millon dollar
- Average duration of the movie must be 114 minutes
- Genre must be : Comedy, Drama, Action, Thriller

These are some of many characteristics which can make a movie profitable,one key point to be noted is  that all the numerical results for the most part are the outcome of the analysis performed on the profit(.=60 million) based dataframe.
