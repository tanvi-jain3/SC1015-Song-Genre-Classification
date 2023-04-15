# SC1015-Song-Genre-Classification
![Green White Creative Tunes Music Festival Canvas Banner](https://user-images.githubusercontent.com/99631047/228569481-1bd250af-63a4-4a61-8672-8423751f36a3.png)


## About:

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on Music from Spotify dataset. Using Music variables (Loudness, Valence, Danceability, Artist name and etc) to predict what genre the music belongs to. For detailed walkthrough, view the source code in this order: 

1: Loading and viewing dataset and Data Cleaning  

2: Data Exploratory Analysis  

3: Machine Learning  


## Problem Statement:

Personalized music recommendation that suits individual preferences are becoming more and more in demand as music continues to be a current trend. Each individual has their own prefences of music. We as a group of data scientists would like to help everyone in enhancing their musical listening experience by predicting music categories using machine learning. To better the music recommendation algorithms, better knowledge of the characteristics of various genres is needed. Users can expand their musical interests from this, in addition to learning about new songs.

This idea could be used in many ways. We could use this to classify songs with ambiguous genres, which could help listeners find songs of their liking. It could also allow users to generate playlists of songs which are similar to ones they already like, leading to an increase in enjoyment and happiness among users. 

## Problem Definition:

* Are we able to predict the genre of a music based on audio features?  
* Which Model would be the best solution to assist with our prediction?
* How accurate is our model in the prediction of song genre?

## Contributors:
Ivan Cheng, Tanvi Jain, Ethan Yeo

## Dataset Description :
We used a dataset from Aneta Kovacheva on Kaggle in different songs. Below is the description of the columns in the dataset.

Name of Variable | Description of variable
--- | --- |
genre | The genre of the song |        
 artist_name| The name of the artist who sang the song |           
 track_name | The name of the song|                    
 popularity | The popularity of the song |                
 acousticness | Acousticness is measured on a scale of 0.0 (not acoustic) to 1.0 (very acoustic). Songs with higher acousticness are more likely to use acoustic and non-electronic instruments. |          
 danceability | Danceability quantifies how suitable a track is for dancing based on a combination of musical elements, like tempo, rhythm, and beat. Songs with higher danceability have stronger and more regular beats. Like acousticness, danceability is measured on a scale of 0.0 (low danceability) to 1.0 (high danceability). |              
 energy | Energy measures the perceived intensity and activity of a song. Energy is also measured on a scale of 0.0 (low energy) to 1.0 (high energy). Songs with higher energy are more intense, dynamic, and loud. |         
 popularity | The popularity of the song |      |                  
 instrumentalness | Instrumentalness predicts whether a track contains vocals. Instrumentalness is measured on a scale of 0.0 (likely contains vocal content) to 1.0 (likely contains no vocal content). Songs with higher instrumentalness are less likely to have vocals. |          
 key | The key in which the song was written. |
liveness | This variable detects the presence of an audience in the song. Liveness is also measured on a scale of 0.0 (no audience) to 1.0 (audible audience). Songs with higher liveness are more likely to have been performed live.|
loudness | Loudness measures the decibel level of a song. Decibels are relative to a reference value, so songs with lower loudness values are quieter relative to the reference value of 0. | 
mode | Whether the song is in a Major or Minor scale | 
speechiness | Speechiness measures the presence of spoken words in a song. It is measured on a scale of 0.0 (low speechiness) to 1.0 (high speechiness). Songs with higher speechiness are mostly composed of spoken words, like poetry or a talk show.  | 
tempo | Tempo measures the beats per minute (bpm) of a song. Many popular songs range from 50 bpm to 200 bpm. Songs with higher tempo have a faster pace. |
valence | valence measures the positivity of a song. It is measured on a scale from 0.0 (low valence) to 1.0 (high valence). Songs with higher valence sound happier and more cheerful.| 

## Models Used:
1) Multi-Variate Decision Tree
2) Random Forest Classifier

## Conclusion:
Upon generating boxplots for the numeric variables against the genre, we learnt that popularity is the variable with the most influence on the genre of the song. This means that different genres of music enjoy different levels of popularity, with the median for the boxplot being highest for hip-hop and pop. This gives us insight into the listening habits of our generation : that we enjoy pop and hip-hop over lower-ranking genres such as Classical Music. 

* Popularity is the variable with the most influence on the genre of the song.
* Different genres of music enjoy different levels of popularity, with the median for the boxplot being highest for hip-hop and pop.
* Accuracy of our models was more when we used a dataset with fewer genres as opposed to one with a lot more.
* Using more predictors gave us a more accurate result. 
* Using K-Cross Validation and GridSearch CV improved the accuracy of our models significantly.
* Random forest classifiers generated a better outcome than decision tree with train 66% and test 56% music genres correctly classified.
* Managed to get above 0.5% accuracy for both test and train datasets which show that although it may not be the most optimal model to classify song genre, it is still accurate on average. 
* Hence, It is possible to predict the genre of a song using its auditory characteristics. However, there are more to be explored.



## Learning Points:

* Collaborating with others using GitHub.
* Implementation of Chi-Square test, using p-values to measure the correlation between two categorical variables.
* The use of K-Cross Validation to determine the optimal depth of a tree that should be used to provide the most accurate results.
* Encoding categorical variables.
* How to predict a categorical variable using both numeric and categorical predictors.
* Usage of Random Forest Classifier from SKLearn.
* Handling an unclean dataset with irregular values.


## References:
1. [Explanation for zero value of probability of chi-square hypothesis](https://datascience.stackexchange.com/questions/107183/p-value-of-chi-squared-test-is-exactly-0-0)
2. [Dataset](https://www.kaggle.com/datasets/vicsuperman/prediction-of-music-genre)
3. [Grid Search and Cross-Validation](https://towardsdatascience.com/cross-validation-and-grid-search-efa64b127c1b) 
4. [Label Encoding](https://towardsdatascience.com/categorical-encoding-using-label-encoding-and-one-hot-encoder-911ef77fb5bd) 
5. [K-Cross validation to find the oiptimal depth of a tree](https://towardsdatascience.com/how-to-find-decision-tree-depth-via-cross-validation-2bf143f0f3d6)




