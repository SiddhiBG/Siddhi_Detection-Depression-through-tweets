
This repo dedicated to the depression detection by using Tweets of the users:

There are two kind of tweets that are required at this project: random tweets that do not indicate depression and tweets that shows the user may have the depression.

The random tweets dataset could be download from the kaggle website by the following link:https://www.kaggle.com/ywang311/twitter-sentiment/data.

Since there is no public dataset exists regardingthe depressive tweets, the essential dataset for this project taken by the websraper with the name of TWINT using the keyword depression by scraping all tweets in an one day span. The tweets which taken as the result of the scrapper may contain tweets that do not shows the user have the depression,such as tweets such as tweets linking to articles about depression. Hence, the scrapped tweets need to be manually check for the better testing results. THe mentioned result is saved as the csv format with the name of "depressive_tweets_processed.csv"

We also need the pretrained vectors for word2Vec model which provide by the google by using the following link: https://drive.google.com/uc?id=0B7XkCwpI5KDYNlNUTTlSS21pQmM&export=download

In this project I used the LSTM+CNN, the model takes in an input and then outputs a single number representing the probability that the tweet indicates depression. The model takes in each input sentence, replace it with it's embeddings, then run the new embedding vector through a convolutional layer. CNNs are excellent at learning spatial structure from data, the convolutional layer takes advantage of that and learn some structure from the sequential data then pass into a standard LSTM layer. Last but not least, the output of the LSTM layer is fed into a standard Dense model for prediction.



![52536100-5a7ba200-2d56-11e9-8f4c-d6d14c96b9ac](https://github.com/SiddhiBG/Siddhi_Detection-Depression-through-tweets/assets/86585405/fafabde3-acaa-4d17-bdb5-f9075e9cfa25)

![52536102-5a7ba200-2d56-11e9-96e9-b00107c1c633](https://github.com/SiddhiBG/Siddhi_Detection-Depression-through-tweets/assets/86585405/fa2347d8-860f-4b4c-9aea-e9597c855c46)

