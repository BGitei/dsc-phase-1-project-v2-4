# Introduction

## Overview

The project aims to use data analysis to help Microsoft enter and succeed in the movie industry by identifying the best types of films to create through exploratory data analysis.

## Objectives

### General Objectives

Analyze successful movie genres at the box office and using findings to decide which types of movies to make.

### Specific Objectives

* Loading datasets into pandas
* Retrieving data from a DataFrame
* Data preparation and cleaning
* Exploratory analysis
* Data visualization

## Questions to be researched

This analysis answers the following questions:

 * What are the most popular movie genres in the box office?
 * What are the most popular studios in terms of movie ratings?
 * What are the movies with the highest worldwide gross?
 * Does popularity affect the total gross?
 * Does the budget affect revenue?
 * Does the ratings affect revenue?
 
# Data Processing
 
## Datasets
 
The datasets are stored in the zippedData folder. The data sources are: 

   1. bom.movie_gross.csv (Box Office MojoLinks)
   2. im.db (IMDBLinks)
   3. rt.movie_info.tsv (Rotten TomatoesLinks)
   4. tmdb.movies.csv (TheMovieDBLinks)
   5. tn.movie_budgets.csv (The Numbers)

## Importing the relevant libraries

Begin by importing all necessary libraries i.e pandas, numpy, cvs, sqlite3 among others.

Also import data visualization tools i.e matplotlib.pyplot as plt and seaborn as sns

### Loading datasets

The following datasets are datasets containing information about the movie industry in general i.e budgets, revenues, reviews, ratings and much more.

To load datasets use the following:
    
 1. movies_budget = pd.read_csv('zippedData/tn.movie_budgets.csv')
 2. movies_gross = pd.read_csv('zippedData/bom.movie_gross.csv')
 3. tmdb = pd.read_csv('zippedData/tmdb.movies.csv',index_col=0)
 4. reviews = pd.read_csv('zippedData/rt.reviews.tsv',     delimiter='\t',encoding='unicode_escape')
 5. conn = sqlite3.connect('zippedData/im.db')
 6. movie_info = pd.read_csv('zippedData/rt.movie_info.tsv', delimiter ='\t', encoding='unicode_escape' )

After exploring and analysing data the following results were yielded to answer the business questions.

## Data Visualization
What are the popular genres in the box office?

![Genres Vs Popularity](https://github.com/BGitei/dsc-phase-1-project-v2-4/assets/163979278/14c292b0-4549-40aa-8fd6-bdcebe92e0e1)

What are the most popular studios in terms of movie ratings?

![Movies Vs Ratings per studio](https://github.com/BGitei/dsc-phase-1-project-v2-4/assets/163979278/ec34ce8d-e46e-48ff-aad2-d9f3163922f1)

What are the movies with the highest worldwide gross?

![Movies Vs Worldwide gross](https://github.com/BGitei/dsc-phase-1-project-v2-4/assets/163979278/f204f3ab-bf15-419f-8bcb-aa5af12af046)

Does popularity affect total gross?

![Popularity vs Worldwide gross](https://github.com/BGitei/dsc-phase-1-project-v2-4/assets/163979278/adfdc7dd-9237-4902-81c0-06fb981924c2)

Does the budget affect revenues?

![Budget vs Revenue](https://github.com/BGitei/dsc-phase-1-project-v2-4/assets/163979278/80672a39-c6c8-4791-8364-18843cc4d7ce)

Does the ratings affect revenues?

![Ratings vs Revenue](https://github.com/BGitei/dsc-phase-1-project-v2-4/assets/163979278/559b91f6-0fd2-4d6f-85cf-ff9f7a0a8d33)

# Conclusion

1. The most popular genres to produce are Drama, comedy and Action movies.
2. The biggest competitor studio is BV in terms of movie ratings and gross revenues.
3. The movies with a high budget also get higher revenues.
4. The movies with a higher rating also have a high gross revenue.

# Recommendation

1. Microsoft should aim to produce drama, comedy or action movies.
2. Microsoft can strive to learn from BV as the best performing studio.
3. Microsoft should also invest a sizeable budget since the higher the budget the more the gross revenue.



