# Web-based-news-aggregation-platform

In today’s scenario there is a huge amount of news content present online there are thousands of
news channels and news site portals where there are millions of articles . Today everyone is busy
and has less time to read news articles and also get confused between which news site to choose
and which is the more reliable source . This project is a step to solve this problem and so we
developed a news aggregator web application on which a user once registered can see snippets of
articles from top news sources and can also choose from categories available
 
 
![image](https://user-images.githubusercontent.com/52206701/115846824-ebbf2680-a43f-11eb-9dd6-b6b93d1b80cc.png)


Backend:-
○ Django (3.1.6)
○ Django-rest-framework(3.12.2)
○ Django-rest-auth(2.1.3)
○ PyJWT
○ Redis
○ PostgreSQL

● Frontend:-
○ Vuejs
○ Vuetify/UI
○ Axios
○ JWT

● News Scraping:-
○ BeautifulSoup
○ Celery
○ Rabbit/MQTT Server

● Deep Learning:-
○ Tensorflow
○ Flask
○ Keras,Sklearn
○ Numpy,Pandas
○ Google Colab training



# Text Classification

The task is to classify the news articles into one of the five categories
◆ The data is first sent to embedding layer which creates the word embeddings
◆ Now these embeddings are sent to RNN cells to extract features if the data
◆ Further the resultant word vector are weighted and summed and then passed to
fully connected layers for classification purpose
◆ Dropout is added to both after RNN and fully connected layer
◆ L2 regularization is employed for fully connected layer weights
◆ We used GloVe embeddings(300d) weights for embedding layer
◆ We used adam optimizer and added early stopping to optimize network weights
◆ The articles are then parse through Deep learning algorithm to get the categories
◆ We created a flask api for prediction which takes list of news articles as input and
returns classes as numpy array

![image](https://user-images.githubusercontent.com/52206701/115847103-393b9380-a440-11eb-84f9-f52c863e83fe.png)



# Future Enhancements
The classification of the news articles could be expanded to multi-label text articles, as
there are many news articles that do not belong to a single category and are instead a
mixture of various categories. Being able to classify multi-label articles will provide
added advantage to the classifiers.Also systems like news articles recommender can be
implemented to test the efficiency of the underlying classifier algorithms and also help
users to enjoy a hassle free and better reading experience.


Try it out here: https://colab.research.google.com/drive/1HUWJuFNBZzTebgVplXx4snJEn0cmaUku?usp=sharing
