# Blake Zurman  
**Scripting for Data Analysis Project**  
**Date**: 12/12/2024  

## Song Sentiment Analysis and Musical Elements  

### Project Overview  
This project explores the relationship between the musical elements of popular songs and their lyrical sentiment. Using CSV files and JSON data from the Genius API, I analyzed songs by artists like Drake, Coldplay, and Post Malone to uncover potential trends and patterns in music and sentiment.

### Data Sources  
1. **3000_spotify_songs.csv** (Retrieved from Kaggle)  
2. **spotify_data_2017_2021.csv** (Retrieved from Kaggle)  
3. **JSON Lyric Data** (Pulled dynamically from the Genius API)  

### Preprocessing  
- **CSV Data**: Cleaned and processed to compute average weekly ranks, allowing for popularity-based ranking of songs.  
- **API Data**: Utilized a Python script to search the Genius API for song and artist details, extracting results into a pandas DataFrame for analysis.  

### Analysis Goals  
1. Do popular songs exhibit a relationship between lyrical sentiment and musical elements?  
2. Do certain artists have a signature combination of musicality and sentiment?  
3. Does sentiment analysis work effectively for modern music?  

### Methodology  
1. Preprocessed data to focus on relevant and popular songs.  
2. Developed functions to pull song and artist data from CSVs and the Genius API.  
3. Performed sentiment analysis using Vader and generated visualizations (e.g., word clouds).  
4. Compared sentiment analysis results with musical elements like danceability, energy, tempo, and valence.  

### Key Findings  
#### Coldplay - *Orphans*  
- **Music Elements**: Danceable, high energy, moderately fast tempo (108 bpm).  
- **Sentiment**: Positive (compound score: 0.98).  

#### Coldplay - *Yellow*  
- **Music Elements**: High energy but slow tempo (67 bpm after adjustment).  
- **Sentiment**: Positive (compound score: 0.97) – **Vader misinterpreted melancholy lyrics.**  

#### Post Malone - *Circles*  
- **Music Elements**: Highly danceable and upbeat, resembling House Music.  
- **Sentiment**: Positive (compound score: 0.96).  

#### Drake - *God’s Plan*  
- **Music Elements**: Extremely danceable, moderate energy, and upbeat tempo.  
- **Sentiment**: Positive (compound score: 0.99).  

### Insights  
- Sentiment analysis can struggle with metaphors, slang, and figurative language in lyrics.  
- Musical elements like tempo, danceability, and energy often correlate with perceived positivity.  
- Combining multiple data sources and analysis techniques in Python led to meaningful insights about music and sentiment.  

### Conclusion  
This project was an engaging exploration of combining CSV and API data to analyze music and sentiment. The process showcased Python's versatility in handling different data formats and performing sentiment analysis, ranking, and visualization.  

### Tools and Technologies  
- **Programming Language**: Python  
- **Libraries**: pandas, Vader (Sentiment Analysis), wordcloud  
- **APIs**: Genius API  
