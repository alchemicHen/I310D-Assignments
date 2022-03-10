__Content warning: the Perspective API is designed for use in content moderation, and the dataset contained very “toxic” comments. Some of the comments in this dataset are racist, sexist, ableist, and offensive. Some comments contain profane language. The particular analysis in the dataset is of high scoring and thus comments considered toxic.__

This project involves analysis of the Perspective API. The [A2_bias_eda.ipynb](A2_bias_eda.ipynb) notebook contains the main analysis.

The [template](Assignment%202%20Template.ipynb) and [pre-labeled dataset](labeled_and_scored_comments.csv) were provided by the class, which contain a template for querying the Perspective API as well as a dataset that contains scores of comments as well as labels attributed to the comments.

An initial exploration of the labeled dataset was done, finding any potential correlation between labels, the count of each particular label, and the most frequent words used for the labels and high-scoring comments.

The hypothesis for analysis was that individual words would query in the API as neutral, even if they appeared in the most commonly used words in high-scoring comments or labels. This is because the Perspective API's machine learning and natural language processing likely considers a phrase's context when assigning scores.

Ultimately, individual words that seemed neutral were indeed neutral in a separate query, even if they did appear in commonly used words in toxic comments. Curse words and profanity continued to return high scores. Phrases containing high scoring words also continued to return high scores, likely because high scoring words apply upward pressure on the scores of the words surrounding it.