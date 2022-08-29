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
Id      | Spotify track ID. |  | 
Title | Title of the track. |  | 
All_artists | All artists featured on the track. |  | 
Popularity | Spotify's popularity rating. It's based on number of plays and how recent they are. |  | 
Release_date | Date when the track was first released. |  | 
Danceability | Danceability describes how suitable a track is for dancing based on a combination of elements such as tempo, rhythm stability, beat strength. |  | 
Energy | Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. |  | 
Key | The key the track is in. |  | 
Loudness | The loudness of a track in decibels (dB). |  | 
Mode | Detects the modal quality of a track, if the song uses major or minor scale. |  | 
Acousticness | A measure from 0.0 to 1.0 of whether the track is acoustic. |  | 
Instrumentalness | Predicts whether a track contains no vocals. |  | 
Liveness | Detects live recordings. |  | 
Valence | A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. |  |  
Tempo | The overall tempo of a track in beats per minute (BPM). |  | 
Duration_ms | Duration of the song in miliseconds. |  | 
Time_signature | The time signature notes how many beats are in each measure of a piece of music. |  | 