# Data-mining-Project
�

Title: Mood-Based Song Recommender System 
1. Introduction 
Objective: 
The goal of this project is to develop a mood-based music 
recommendation system using audio features from songs. By 
analysing various features such as valence, energy, danceability, 
and others, the system aims to suggest songs that align with a 
user’s current mood. 
2. Dataset Description 
Source: 
Spotify audio features dataset. 
Columns Used: 
 genre, artist name, track name, trackside 
 popularity, acoustic Ness, danceability, durations, energy 
 instrumental Ness, key, liveness, loudness, mode 
 speckiness, tempo, time signature, valence 
Key Mood Indicators: 
 Valence: Positivity of the song (happy vs sad) 
 Energy: Intensity and activity 
 Danceability: How suitable a track is for dancing 
3. Methodology / Procedure 
Step 1: Data Preprocessing 
 Loaded the dataset using pandas. 
 Removed duplicates and missing values. 
 Scaled numerical features using MinMaxScaler. 
Step 2: Mood Classification (Optional) 
 Divided moods based on valence and energy: 
o Happy (high valence, high energy) 
o Sad (low valence, low energy) 
o Calm (high valence, low energy) 
o Angry (low valence, high energy) 
Step 3: Clustering 
 Applied Means Clustering to group songs into clusters 
representing similar mood/energy types. 
 Chose an optimal number of clusters using the Elbow 
Method. 
Step 4: Recommendation System 
 Given a mood (happy/sad/calm/angry), recommend top 
songs from the closest matching cluster. 
 Used cosine similarity or nearest neighbours for fine-tuning 
recommendations within clusters. 
4. Results 
 The dataset was successfully clustered into mood-based 
groups. 
 Sample outputs include song recommendations for each 
mood type. 
 The system effectively recommends songs that align with 
mood-based preferences by analysing key features like 
valence, energy, and danceability. 
5. Conclusion 
This project demonstrates how audio features can be used to 
create a personalized music recommendation system based on 
mood. It integrates feature engineering, clustering, and basic 
recommendation logic to provide useful suggestions. 
Future Work: 
 Incorporate user feedback for personalized tuning. 
 Integrate with a streaming service API (e.g., Spotify API). 
 Apply deep learning techniques for enhanced modelling.
