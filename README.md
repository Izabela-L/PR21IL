# My music taste: A data analysis
## Description of the problem
The field of my research is music. I wanted to anaylze my music taste with the help of datamining. I want to see if it is possible to isolate distinctive features in the genres and artists I gravitate towards. The main goal of this project is to:
* get better insight into my music taste
* find trends and patterns in my listening habits
* discover how diverse (or homogenous) my taste is
* learn which musical properties influence my liking of a song
* draw a comparison with another user
## Data
I have chosen to scrape the data from my Spotify account. Scraping was done using the Spotify Web API and Spotipy. Spotipy is a Python library that makes it easier to access different end points in the API. Spotify was a clear choice because they collect vast amounts of metadata for music, as well as a lot of information on their users. The end result of my web scraping is the library.csv dataset. 

In addition to scraping information from my personal library, I also collected data from a random user. I searched for a playlist of a similar size that contains another person's music library and collected the same attributes. This is the randomuser.csv dataset.
### Data attributes

Both the library.csv dataset and randomuser.csv consist of track metadata and Spotify's audio features for each of the songs.

Attribute | Description      | Type | Value
----------|------------------|------|------
Id      | Spotify track ID. | String | Discrete
Title | Title of the track. | String | Discrete
All_artists | All artists featured on the track. | String | Discrete
Popularity | Spotify's popularity rating. It's based on number of plays and how recent they are. | Numeric | Discrete
Release_date | Year when the track was first released. | String | Discrete
Danceability | Danceability describes how suitable a track is for dancing based on a combination of elements such as tempo, rhythm stability, beat strength. | Numeric | Continuous
Energy | Energy is a measure that represent intensity and activity. | Numeric | Continuous
Key | The key the track is in. | Numeric | Discrete
Loudness | The loudness of a track in decibels (dB). | Numeric | Continuous
Mode | Detects the modal quality of a track, if the song uses major or minor scale. | Categorical | Binary
Acousticness | Detects whether the track is acoustic. | Numeric | Continuous
Instrumentalness | Predicts whether a track contains no vocals. | Numeric | Continuous
Liveness | Detects live recordings. | Numeric | Continuous
Valence | A measure describing the musical positiveness conveyed by a track. | Numeric | Continuous
Tempo | The overall tempo of a track in beats per minute (BPM). | Numeric | Continuous
Duration_ms | Duration of the song in miliseconds. | Numeric | Discrete
Time_signature | The time signature notes how many beats are in each measure of a piece of music. | Numeric | Discrete

