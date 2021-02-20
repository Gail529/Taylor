# Content-based /Mood aware Recommendation system for Taylor Swift's Songs

Created a recommendation engine that recommends a Taylor Swift song based on the mood of the user.
- Gathered audio features such as (danceability and popularity) from the Spotify API.
- Scraped song lyrics from the web using Beautiful Soup.
- Made use of the NRC emotion lexicon to analyse the emotions expressed by the message of the song.
- Generated emotion scores for the lyrics of each song in the dataset.
- Used the audio features together with the emotion scores as the final set of features.
- Generated song recommendations using Cosine Similarity.
- Created a simple Streamlit Application to test out the engine.


