# Content-based /Mood aware Recommendation system for Taylor Swift's Songs

Created a recommendation engine that recommends a Taylor Swift song based on the mood of the user.
- Gathered audio features such as (danceability and popularity) from the Spotify API.
- Scraped song lyrics from the web using Beautiful Soup.
- Made use of the NRC emotion lexicon to analyse the emotions expressed by the message of the song.
- Generated emotion scores for the lyrics of each song in the dataset.
- Used the audio features together with the emotion scores as the final set of features.
- Generated song recommendations using Cosine Similarity.
- Created a simple Streamlit Application to test out the engine.

# Project Walkthrough :Data Collection
metadata.ipynb -
Fetched Taylor Swift's music data using Spotipy a python library for the Spotify Web API.The audio features provided by the
API include:
- acousticness
- danceability	
- energy	
- instrumentalness	
- liveness	
- loudness	
- speechiness	
- tempo	
- valence	
- popularity

taylor_lyrics.ipynb-
Fetched the song lyrics from the 6 most recent Taylor Swift albums namely RED,1989,REPUTATION,LOVER,FOLKLORE,EVERMORE, using beautiful soup.

# Data preprocessing
emotions.ipynb -
To Clean the lyrics I perfomed whitespace,punctuation,numbers and stopwords removal, lowercasing ,tokenisation  and lemmatisation.Using nltk and  pandas.
# Feature engineering
emotions.ipynb -
Using The NRC emotion lexicon I created a dataframe showing the emotional inclination of each song against 8 emotions namely Anger	Anticipation	Disgust	Fear Joy Sadness	Surprise	Trust.I then merged the audio features with the emotion scores into one dataframe.
# Making Recommendations
Generated item-item based recommendations using Cosine Similarity.Created a simple streamlit app to interact with the Recommendation engine.


