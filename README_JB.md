## Project 3: Web APIs & Classification - Executive Summary
### Problem Statement
HHired by a leading plant-based delivery service who wants to understand through Natural Language Processing (NLP) the posts of two subreddit communities to gain insights for a more data-driven marketing campaign.

In order to address their problem, I have collected data from posts from two subreddit communities (r/plant-based and r/ vegan) to analyze and identify themes about the posts and which subreddit posts are coming from.

        
### Process

Process:

Data Collection:
Used Pushshift.io for collecting data on r/plant-based and r/vegan posts.
Collected 1,000 posts from each subreddit
Removed unnecessary columns and kept relevant columns including, posts,  number of comments, and author

Data Cleaning and EDA
Conducted data cleaning and EDA.
Preliminary EDA showed many similarities between the two subreddits

PreProcessing 
Used Count Vectorizer and TFIDF Vectorizer to transform text to numerical features
Removed stop words to focus on important words.

Modeling / Evaluation

Developed/Evaluated Models 
Split the data into training and testing for validation
Baseline Accuracy Score
Multinomial Naïve Bayes
Random Forest


## Conclusions / Recommendations

While all models, performed better than the baseline accuracy score of 0.50, the Random Forest model with TfidfVectorizer has the best predictive performance on this classification problem.
Max_features as 1000 which is the smallest number among the max_features parameters tested for, and n_gram range as 1-2, which prefers up to two-words and the removal of stop words.

There was measurable increase in the predictive performance of all models compared to the baseline accuracy.
However, similarities between vegan and plant-based subreddits were challenging for the models and resulted in relatively low accuracy scores.
Next steps include, exploring other relevant subreddits; collecting more training data; doing more pre-processing (e.g., removing more stop words); conducting sentiment analysis; and trying additional models like boosting and K-Nearest Neighbors.


