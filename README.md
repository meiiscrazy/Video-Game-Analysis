# Video-Game-Analysis

## Presentation
- https://docs.google.com/presentation/d/1yCDlBEnNzUETAqg6hw0UhwyvKmxIxOfuXmUYwiyt2jw/edit?usp=sharing

## Final Presentation and Recording
- https://docs.google.com/presentation/d/1F2vPbk1FQwRawPsIchmNKKqJq2pdLOP85Ex46gSOpLg/edit?usp=sharing

- https://drive.google.com/file/d/1qHSxrrQ663Appq8pMvxjKv4cvjxaryq_/view?usp=sharing

## Tableau Dashboard
https://public.tableau.com/profile/betsy1119#!/vizhome/SteamStory/Story1?publish=yes

## Overview
Analyze video game sales and performance through the creation of a dashboard using analysis of ratings, owners, sales, playtime, and release dates. 
Use machine learning models to predict the success of a game based on critic score and positive user ratings or sales. 

## Reason Why
During a March 2020 survey, video gamers in the United States reported that they spent 45 percent more time playing video games amid the quarantine than in the previous week.
This has impacted the way video game industries strive to appeal to its consumers, with free to play, cross platform and phone games increasing in popularity amongst consumers of all expertise levels and ages. 
Our aspiration is that this project will shine some light in terms of users looking for games to get started in either playing or for companies to find some of this analysis of worth to optimize video game sales based on user and critic scores.


## Description of the Data
We're using data from Steam, this data includes the game name, date released, user ratings, genre, price, and more. We will be including charts/graphs/tables to visualize our data. We will also be using this data as our base for our machine learning model. The goal of the machine learning model is to predict what genre will be popular in the upcoming months. 

Source: [Source 1](https://www.kaggle.com/nikdavis/steam-store-games)
As a preliminary data preparation and exploration, Kaggle data from a Steam API call includes data for different types of games along with the amount of owners, ratings, price, whether the game is in English or not, categories for each games as well as genre types associated with each game. Other information included developer, platform, and publisher information.

Source: [Source 2](https://www.kaggle.com/ashaheedq/video-games-sales-2019)
A second source focused on sales for each game has been used to create a number of visualizations related to the success of sales across a variety of categories such as rank, name, publisher, developer, critic and user scores, as well as total shipped units, global sales and the year release of the game. 

## Questions we Hope to Answer
- What types of games are currently successful?
- What types of games are successful?
- How can a person new to Steam or video games in general narrow their search to find a video game they will enjoy playing?
- How can free to play games be compared to paid games and how can that help users identify which games to play based on their budget?

## Data Exploration Explanation
Steam Data
Steam API data was used to determine relationships between ratings, owners and what the current Steam system provides for its users. Through analysis of Steam data, we reinforce understanding of what genres have performed well, what years have proved successful for Steam game sale, genres that are currently on the rise, as well as games that have a good user standing in terms of positive rating reviews, playtime and price. We can also identify what games to play based on the average rating and price!

## Global Sales
Global sales data was analysed to determine what genres, publishers, video games are the most successful so far. This dataset also provides a column of critic scores that was compared with global sales to determine a linear regression relationship later used as a preliminary machine learning model. 

## Joined ERD tables using PGAdmin
A joined database is used to merge ratings, global sales, playtime, price, and critic scores since preliminary analysis trends show some correlations between sales and critic scores as well as positive rating ratios. A normalized ratings calculated field is used to be able to trend the average value of each Steam game name to a normalized parameter to trend for linear regression analysis. 

## Machine Learning Model 
Through our analysis, a linear regression model was created preliminarily using the critic score and global sales linear regression trend to create a predictive model.
Additionally, a second linear regression model was also created for positive rating ratio and critic scores. 
Feature selection involved the selection of a positive rating ratio, critic scores and global sales. 
The model currently has an accuracy of 1.0 which shows that the model is overfitted. Some reasons for this could be data normalization or scaling issues. 

## Dashboard Blueprint 
A draft storyboard using Tableau will be created using current video game statistics and how the Steam data relates to each of them. The user will then be able to interact by clicking and scrolling through video game data based on positive and negative reviews to be able to determine what games are budget conscious and most likely to be worth a minimal cost through ratings or critic score based data. 

## Technologies, Tools, Languages 
The technologies used so far have been Github, Tableau, and Jupyter notebooks for preliminary analysis and project tracking. Tableau has been used to create a story board and dashboard compilation of preliminary analysis. Github has been used to track team members' progress and individual project contributions. 
The code throughout the project will use Python, SQL with potential to use Javascript and HTML. 
ML models were analysed and performed using Python, where SQL and PDAdmin was used to join tables and tying the data for analysis to the database. ML models also used Decision Tree coding using TensorFlow. 

## Analysis Conclusions 
- Action games fare better in sales and are also the most searched category/genre
- Ratings and Price show to have a positive relationship
- Playtime provided a good indication on what games were most popular 
- The most used tag within the Steam API were “single-player” followed by “multi-player” then “cross-platform”
- 2013 was the only year in which the amount of owners in video games surpassed 100 million
- Since 2012-2013 the average positive rating ratio of games on Steam has been decreasing. Does this mean video games are not as good as they once were? Is this impacted by the growing demand in phone games and cross-platform games?
- Free to play games are in high demand. When examining the growing trends of genres, it would seem that strategy, free to play games had the most amount of genres with positive rating ratios. 
- Based on the trends seen between critic scores, sales and positive rating ratios it would be good to examine how best to optimize video game price and improve sales based on a game’s rating ratio or critic score.
 
## Future Analysis Improvements
- Improvement of machine learning model to improve video game prices based on specific critic scores and their user ratings 
- Explore other features that might have impact to improve model 
- Find a way to normalize/scale data to have better training and test sets
- Improve the dataset size. We are currently only using data based on appid or game names that have the features we look for.
