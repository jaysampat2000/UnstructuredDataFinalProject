# UnstructuredDataFinalProject

# Web Scraping and Sentiment Analysis of IMDb Reviews: A Report on the Bollywood Movie, “Animal”
# Introduction
The project investigates public sentiment towards the controversial Bollywood film “Animal” using web scraping and sentiment analysis techniques. Known for its polarizing content, “Animal” has been both critiqued for its themes and celebrated for its storytelling, creating a dichotomy between critic opinions and audience ratings. This report aims to bridge the gap by analyzing user-generated content from IMDb reviews to understand the broader audience perception of the film.

# Rationale
The motivation behind this project stems from the stark contrast in reception between critics and the general audience regarding “Animal”. Critics have labeled the film as “cheerfully misogynistic, morally bankrupt, and stomach-churningly violent”, while it still managed to secure a fifth place among the top-grossing Hindi movies. This discrepancy raises questions about the factors that contribute to a film’s success and the role of audience sentiment in shaping its reception. By applying web scraping and sentiment analysis, this project seeks to uncover the underlying sentiments and themes that resonate with the audience.

# Methods
# Data Collection
The data was collected using the playwright library to automate web scraping on IMDb’s review section for “Animal”. The script navigated through the website, interacted with the “Load More” button to reveal additional reviews, and extracted the review texts and user ratings. These were then compiled into a Pandas DataFrame for further processing.

# Data Cleaning and Preprocessing
The raw review comments underwent a series of cleaning steps to prepare them for analysis. This included converting texts to lowercase, removing punctuation and numbers, stripping whitespace, and lemmatizing words. Additionally, stopwords were removed to reduce noise and focus on the more meaningful content within the reviews.

# Sentiment Analysis
Using the cleaned review texts, sentiment analysis was performed to assign a sentiment polarity score to each review. This score indicates the positive (1) or negative (-1) nature of the text, on that scale. The sentiment scores, along with user ratings, were then analyzed to explore any correlations between the sentiment expressed in reviews and the numerical ratings given by the users.

# Visualization
Various visualizations were created to represent the data, including distribution plots for ratings and sentiment scores, and word clouds to visually depict the most frequent and significant words used in the reviews.

# Findings
# Polarization in Ratings
The initial exploration of the ratings revealed a significant polarization, with the majority of ratings being either 1 or 10. This suggests a divided audience reception, with some viewers highly appreciating the film, while others strongly disliked it.

# Positive Sentiment Skew
Despite the polarization in ratings, sentiment analysis revealed a positive skew in sentiment scores, with a mean score of 0.1 indicating a generally positive sentiment among the reviews. This suggests that, on balance, the audience’s textual feedback on “Animal” leans more towards the positive.

# Word Cloud Insights
The word clouds highlighted a focus on “positive” words like “story” and “character”, overshadowing negative terms such as “bad” and “violence”. This indicates that despite the film’s controversial themes, elements like storytelling and character development were appreciated by the viewers.

# Correlation Analysis
The sentiment scores alone were found to be a weak predictor of the user ratings (0.225), indicating that while sentiment provides insight into the qualitative reception of the film, it does not directly translate to the quantitative ratings.

# Conclusion
The report reveals a complex audience reception towards “Animal”. Despite significant criticism and majority 1-star ratings, the overall positive sentiment and appreciation for certain aspects of the film suggest that it managed to resonate with a substantial portion of its viewers. This report highlights the nuanced relationship between audience sentiment, critical reception, and commercial success, suggesting that films capable of evoking strong emotions, regardless of their nature, can achieve notable engagement and discussion among viewers and make a ton of money. However, it sets a dangerous precedent going forward for Bollywood and we must be careful as Bollywood movie viewers to not embody such behaviors in real life.
