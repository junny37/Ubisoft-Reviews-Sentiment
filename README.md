<img src="http://imgur.com/1ZcRyrc.png" style="float: left; margin: 20px; height: 55px">

# Project 3: NLP & APIs


## Background & Problem Statement
---

[Ubisoft](https://www.ubisoft.com/en-us/company/about-us) is a leading company in the gaming industry. Some [popular games](https://www.thegamer.com/ubisoft-best-games/#assassin-rsquo-s-creed-4-black-flag) include the famous Assassin's Creed series, Far Cry, Tom Clancy, as well as Rayman, just to name a few. Ubisoft has been developing a new game over the past couple of years, called "Skull & Bones". This upcoming game was [inspired by their most popular Assassin's Creed series, "Assassin's Creed IV: Black Flag"](https://screenrant.com/skull-and-bones-best-game-recommendations/).

Posing as someone who is working for Ubisoft's data team, I am interested in identifying reviews for Assassin's Creed IV: Black Flag, and classifying whether they are positive or negative. This is so we can use this model in the future, to further analyse which part of the game people liked and disliked, so Ubisoft can further improve the game, as well as include and improve the appropriate elements for their upcoming Skull & Bones game. 

For now, <font color = 'green'>**the aim is to create a model that is able to perform sentiment analysis on Assassin's Creed IV: Black Flag steam reviews**</font>.

For this project in particular, I will be using Naive Bayes and Random Forest classifiers as the developing models to perform the sentiment analysis. Since the data that was retrieved from Steam does have a column on whether the user would or would not recommend the game, we will use that as a comparison on how well the model performed.


## Data Dictionary
---

|Feature|Type|Description|
|---|---|---|
|num_games_owned|int|number of games owned by the user|
|num_reviews|int|number of reviews returned in this response|
|playtime_at_review|float|playtime when the review was written|
|last_played|datetime|time for when the user last played|
|review|object|text of written review|
|timestamp_created|datetime|date the review was created|
|voted_up|int|1 means it was a positive recommendation|
|votes_up|int|the number of users that found this review helpful|
|votes_funny|int|the number of users that found this review funny|
|weighted_vote_score|float|helpfulness score|
|comment_count|int|number of comments posted on this review|


## Analysis & Conclusions Summary
---

As part of Ubisoft's data team, we were able to produce a 99% accurate model to predict the positive and negative reviews from Steam. This is using the Random Forest model. 

The model, although performs very well, can always be improved. Other areas to try could be to increase the features to see if this gives an ever more accurate result.

Ubisoft's Assassin's Creed IV: Black Flag had received an overwhelming number of positive reviews and recommendations, and the model developed was able to filter through these reviews to classify them as positive and negative in a successful manner. 

This will help Ubisoft in the future endavours to identify what users liked and what to improve on, for both their current Assassin's Creed IV: Black Flag game, as well as their development of Skull & Bones.