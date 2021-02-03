# Week 4: Mini Group Assignment
by Pawan (Sine) Polcharoen and Claire Guo

## Project Title: Global Music Trends

Read our project proposal [here](https://github.com/spolcharoen/DH140_Project/blob/main/Project_Proposal.md).

## Roles
In our group project, our titles are both Project Co-Leads. However, we have smaller roles assigned within the group. Specifically, Sine will be primarily in charge of creating charts from the datasets. She also will be exploring the May 2020 data set this week. On the other hand, Claire will be primarily in charge of visualizing the data spatially through using maps. She will also be exploring the June 2019 data set this week. We both plan on checking base after completing our individual analysis on the 2020 and 2019 data sets. Both of us plan on splitting up work evenly on future write-ups, research, and searched for additional datasets to gain a deeper understanding of how different global factors affect music preferences.

## Status Update
So far, the team has felt confident in the data sets we have found for the project and we have a good idea of what we want to explore in the initial data exploration. However, we are still exploring the ‘why’ factor for our project and are looking to explore more data to see if global music preferences are affected by economic or political differences. We got the idea for this connection from [this article](https://www.researchgate.net/publication/323612124_The_geography_of_music_preferences). Although the article focuses on a national level, we hope to analyze the pattern on a global scale. For now, we found that the national census data project we completed last is not directly related or helpful for our project, but we plan on analyzing global census data instead to get a broader understanding of global demographics.

## Data Update
From our three original data sets, we have joined the genres data to both the May 2020 and the 2017-2019 Spotify data sets. The 2017-2019 spotify data set we initially had contained over 8 million observations. Thus, we had to cut down the data set significantly in order to work with it in Jupyter Notebook. To do this, we subsetted the data to only include observations from June 2019. With this reduced data, we could then conduct an inner join with the genres data set to create a data set with around 300,000 observations (spotify_june2019.csv -- this file was too large to upload to GitHub). We did the same join with the genres data and the May 2020 data, which was already small enough to work with ([spotify_may2020.csv](https://github.com/spolcharoen/DH140_Project/blob/main/spotify_may2020.csv)). Presently, we are doing explorations on both data sets with the goal to eventually choose just one.

Furthermore, we are also exploring [global census data](https://github.com/yohman/world-projections/blob/main/world.geojson), specifically looking at profiles regarding economic and political differences. In the coming weeks, we plan to use our new joined data in conjunction with the census data to analyze how global music trends are potentially affected through economic and political discourse. 

## Concerns:
### Major Concerns
We have two major concerns. The first concern we have is solidifying the ‘why’ aspect of our research. We hope to have a clearer understanding of this as we explore our data sets and find relationships. Our second concern is about the amount of data we have and the process of cleaning it. As of now, we hope to narrow down which of the two Spotify data sets we will focus on and the variables we want to focus on within the data. We are also worried that there may not be a link between economic and political differences when looking at music trends globally.

### Minor Concerns
A minor concern we have is merging the global census data with the Spotify data. This week, we are looking at our data sets separately, but we are going to have to work on finding that link. Furthermore, we both struggled to figure out how to create maps from a .csv file, so that is something we will need to ask for help with.
