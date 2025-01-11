# EmotionDetection-SongRecommendation
Here is a youtube video of us demonstrating our project : [Presentation](https://youtu.be/-KRTwLfZEj8?si=PN_GSGZZBNgf2sta)
## Datasets

The datasets used as part of this project are -
1. RAVDESS Audio Dataset
2. Spotify top 10k songs
3. Data through Spotify API

## Process
The Audio dataset is first pre-processed using a Mel Spectrogram and is further augmented by adding either noise, stretching or increasing or decreasing the noise.
The emotion detection python notebook enables the user to run the end-to-end process for emotion detection using the audio dataset

The Spotify dataset is used and APIs are leveraged to procure songs based on the URI of the playlist. Clustering is done to classify the songs into one of the 8 emotions obtained from the RAVDESS dataset process

## Modelling
Ensemble of VGG16 and Random Forest is used to predict the emotion. Features are extracted from the VGG 16 and is fed as an input to the Random Forest. For prediction, an unseen audio is used and one of the eight emotions is given as the output.

This output would go as an input to the Spotify process which is clustered using K-means clustering. 
