# Midterm Updated Project Proposal
Pawan (Sine) Polcharoen and Claire Guo

**Access our Midterm presentation slides [here](https://docs.google.com/presentation/d/1iTUqLe8PNnsSGl7mJExCJObC4vA-9hh1BCSEjcLWo44/edit?usp=sharing).**
**Access our Midterm JupyterHub notebook [here](https://github.com/spolcharoen/DH140_Project/blob/main/DH140_Midterm%20(1).ipynb).**

## Introduction
Spotify is an audio streaming platform that is used by millions of artists and listeners across the globe. In our DH140 project, we want to analyze top songs in different countries and what makes them popular. Furthermore, we also want to look at economic differences between countries to see if there are any underlying trends between economic status and music preference. After careful analysis, we hope to answer the following research question:

### What are the characteristics of top songs across the world and how do external factors, such as global economic differences, influence diverse music tastes?

In this project, we look at how global economic differences influence cultures around the world through the lens of diverse music tastes.
Listening to music is a quintessential and universal human activity that plays a role in the formation of culture. Different countries have their own cultures, influences, and popular media, thereby causing people to have diverse music tastes around the world. Music reflects culture and in this project, we hope to analyze factors that influence diverse music tastes on a global scale. More specifically, we want to see how economic productivity in countries influences citizens’ music preferences. This can help explain how the economy of a given country influences citizen life, media, and culture.

Furthermore, we also hope to provide information that Spotify and music artists around the world can use to best market their content. By analyzing what makes certain songs popular in certain countries, artists can understand how to cater their songs to their audiences by learning who their listeners are, where they are from, and what they prefer. Our project supports Spotify in their mission statement:

> “Our mission is to unlock the potential of human creativity – by giving a million creative artists the opportunity to live off their art and billions of fans the opportunity to enjoy and be inspired by it.”

The spatial scope for this project is global. Working through a global lens is important for this project because we want to see how different cultures are expressed through music taste. Furthermore, we want to focus on economic differences between countries and looking at a global scale will allow us to view GDP trends across global regions. Moreover, with Spotify data from June, 2019 and May, 2020 and global GDP data from 2019, we will be able to gain a wide understanding of music trends and economic productivity across many nations.


## Data Sources
We started with 5 main data sources, which we will subset and join for further analysis.

The first dataset contains Spotify’s top 200 songs in each country from 2017 - July 1st, 2019. The data contains the country, date, track, position, track name, artist, and number of streams for each top song.

Spotify music trends: https://www.tableau.com/about/blog/2019/7/how-visualize-spotify-music-trends-tableau

The second dataset contains Spotify’s top songs by country in May 2020. The dataset contains the title, rank, artists, album, duration, country and continent of the top 50 songs by country.

Spotify - Top Songs by Country Charts: https://www.kaggle.com/hkapoor/spotify-top-songs-by-country-may-2020

The third dataset is an analysis of song characteristics, such as speechiness, acousticness, instrumentalness, and liveness, for different kinds of music genres.

Dataset of songs in Spotify: https://www.kaggle.com/mrmorj/dataset-of-songs-in-spotify?select=genres_v2.csv 

The fourth dataset contains the GDP values for 264 countries around the world in 2019.

2019 GDP data: https://drive.google.com/drive/folders/1FiI9kQI_FWoSkbQ4dfiRv3IwdrYX7sZI 

The fifth dataset is a global .geojson file that contains the iso codes and geometry coordinates for 249 countries. 

Global Geojson file: https://github.com/yohman/world-projections/blob/main/world.geojson 

In our project, we intend to create visual maps showing which kinds of songs are popular in each country and construct bar charts for specific countries that break down popular song preferences by their song characteristics. In order to create these visualizations, we have joined the genres data to both the May 2020 and the 2017-2019 Spotify data sets. The 2017-2019 spotify data set we initially had contained over 8 million observations. Thus, we had to cut down the data set significantly in order to work with it in Jupyter Notebook. To do this, we subsetted the data to only include observations from June 2019. With this reduced data, we could then conduct an inner join with the genres data set to create a data set with around 300,000 observations ([spotify_june2019.csv](https://drive.google.com/file/d/1HWuwCSTL682Uo9b44G2VvQYEM2NvqBAf/view?usp=sharing)). We did the same join with the genres data and the May 2020 data, which was already small enough to work with ([spotify_may2020.csv](https://github.com/spolcharoen/DH140_Project/blob/main/spotify_may2020.csv)). By matching each top song with its corresponding genre, we were able to identify which song characteristics were most common amongst popular songs in each country.

Furthermore, we joined the global .geojson dataset to our combined Spotify and song characteristic data to visualize these music preferences spatially. In our current analysis, we created charts for overall global genre differences in June 2019 and May 2020. For the May 2020 data, we created interactive charts that looked at the frequency of top songs at different acousticness levels for each continent. For the June 2019 dataset, we created a similar chart that measured song frequency at different acousticness levels, but grouped by countries instead. We also visualized GDP differences and song characteristic levels for each country using global maps.

In the future, we hope to connect our song characteristics and GDP spatial data to look for any underlying correlation that connects economic productivity to music taste. We also plan on looking at other global factors such as political, educational, racial, and linguitic differences around the world that may also influence music preferences.

## Conclusion
From this research, we hope to better understand how the world listens to music and determine specific factors that influence a country’s music taste and culture. We intend on using Spotify datasets to visualize cultural differences between countries and hope to discover what specific characteristics in songs make them popular in specific countries. We hope to connect this data with global GDP datasets in order to analyze how countries’ economic wealth can influence preferred song characteristics. The data from this project can be used to determine how the economy influences culture, life, and media in countries and how music taste differs by geographic location. Furthermore, by visualizing global music trends, we believe our data can help artists around the world create favorable music for their targeted listeners and help Spotify create better user experiences for their users by recommending favorable music to listeners in different countries.
