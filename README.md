# The Radio Landscape Project

## Introduction

The Radio Landscape Project originated from a personal curiosity during a road trip in August 2022. As I traversed through various regions, I couldn't help but notice the stark differences in radio offerings within just a few dozen miles. This project aims to explore the multifaceted aspects of the radio landscape, including the number of stations available, the diversity of music genres, the types of programming offered (such as news, sports talk, political discourse, religious content), as well as the regional variations in listenership habits. By delving into these nuances, we hope to uncover insights into political, sociological, business, educational, and religious dynamics across different regions.

## Updates

**FEB 6:** Here is my pitch:

The 2024 election holds immense significance for the future of critical issues such as healthcare, immigration, civil rights, equity, climate policy, and geopolitics. However, the oft-repeated adage, "This is the most important election of your life," has become a tired refrain in the political landscape. While I diligently exercise my right to vote in every election - be it national, state, local, or for school board positions - I cannot shake the sense of futility that sometimes accompanies casting my ballot, particularly in national elections.

Not all votes are created equal. The outcomes of presidential elections are largely determined by so-called 'purple' states, leaving voters in solid ‘red’ or ‘blue’ feeling disenfranchised and less motivated to participate in down-ballot races where their impact could be significant. (Credit to fellow John Carroll graduate Tim Russert for the red/blue state labels)

To effect change, the current electoral system requires a substantial overhaul, but achieving this change is contingent upon winning within the existing framework.

In an environment where campaign donations are limited, the efficiency of message delivery becomes paramount. While certain mediums such as online ads, email campaigns, and television advertisements have proven effective in reaching a broad audience, the mere delivery of a message does not guarantee a receptive audience. Many individuals actively avoid content that challenges their beliefs, while others seek to avoid political messaging altogether. Campaigns can tailor messages to different audiences but must exhaust every avenue that can reliably deliver that message in chosen Congressional Districts.

This project aims to explore whether targeted spending on FM radio advertising in selected congressional districts can be optimized by analyzing and leveraging the FM radio landscape within those areas. By examining where voters typically listen to the radio - whether during their commute, at work, or at home - and leveraging data from the FCC and the US Census, I seek to infer the preferences and characteristics of listeners. Through this analysis, I endeavor to provide insights into the potential application of allocating spending on FM radio messaging campaigns. I am excited at the prospect of that application but at the bare minimum, this provides registered owners of each FM station broadcasting into these key districts.

**FEB 6 AM:** I mapped all the congressional districts and 'nearby' stations. Later I plan to use distance, power, and basic height information to infer which stations are dominant for specific locations for each of the available channels.
![screen shot](https://github.com/seanhulseman/FM-Broadcast-Landscape/blob/main/images/all_GA.png?raw=true)

**FEB 5 PM:** Here is a preliminary example plot of a congressional district which contains all FM transmitters (hypothetically)
![screen shot](https://github.com/seanhulseman/FM-Broadcast-Landscape/blob/main/images/GA_01_station_map_ex.png?raw=true)

**FEB 5 AM update:** I can now create buffers of desired size around each district that crudely filter down the number of stations needed. Later I will calculate distance or maybe signal strength for each channel to explore the radio landscape of these example districts.

**FEB 5 AM:** I have reliable congressional map data and 'radio_landscape_3.ipynb' is a Google Colab notebook exploring geopandas. I took some test screenshots of geopandas working and exploring the geodataframe; the data can be found [here](https://drive.google.com/drive/folders/1mAKcFCQt7bf6bRJsn8x-_Bcwo6ULf9pa?usp=sharing).
![screen shot](https://github.com/seanhulseman/FM-Broadcast-Landscape/blob/main/images/congressional_district_gdf_georgia.png?raw=true)

As of January 31st, 2024: Started outlining a project to leverage the FM Landscape for targeted political messaging in key voting areas (precinct, city, county), aiming to reach populations difficult or even resistant to engage through conventional methods. The project is in its early stages, with potential for promising application of data. Updates to README.md and project repository will be added here as progress continues.

## Objectives and Questions

- Investigate the regional variations in radio programming and listenership habits.
- Analyze the impact of radio station diversity on societal and cultural dynamics.
- Explore correlations between radio preferences and sociopolitical factors.
- Examine the implications of commercial vs. educational radio stations on communities.

## Data Collection

The project utilizes data obtained from the FCC FM Radio Query tool, which provides detailed information about radio stations across the United States. After retrieving the raw data, efforts were made to clean and preprocess it, including addressing encoding issues and labeling stations as commercial or educational.

## Dataset Availability

The 'FM_stations_labeled.csv' dataset created from the FCC FM Radio Query is available for public use. Feel free to explore and analyze this dataset, and don't hesitate to contribute to the project by sharing your findings or suggestions.

## Features
* **jupyter notebook 1** - Obtaining the data, label edu and commercial, N/S,D,M,S --->(latitude) and W/E,D,M,S --->(longitude) decimal form for geodatframe later - save the master csv - NO DROPPING HERE What else can I do with the data?
* **jupyter notebook 2** - EDA and Cleaning (NULL ISLAND), UNITS! For the different services - research more on what those mean. Do they need different considerations than others? DA, NA?, FM Status
* **Jupyter notebook 3 (USE GOOGLE COLAB)** - Example use case of the FM Landscape to analyze Congressional Districts in Georgia
* **App** - Interacting with the stations - search a location, hear a station? display stations? Listen to a station? - big owners (IHM ex) may have ways to listen to many stations. the process to find those can be automated??
* **Jupyter Notebook 4** - Modeling - Predict commercial or educational. For census cities, what is the general diversity in radio landscape between those two measures. Can I group the stations further using NLP by company owner? Station description scraped? EDU stations - [College, Religious?, News/Talk?, Music?, grab bag? ,.... ]. Commercial [ genres/music?, major owners and everybody else? News/Talk?,]

## Installation
Geopandas and other geospatial software are a pain to install locally but Google Colab seems to work well enough! Most, if not all, geodataframe work will be done in Google Colab notebooks usable on any device.

## Usage
Make a copy of Colab Notebooks

## Preliminary images
This is a proof showing that my DMS ---> Decimal conversion worked. Without properly dealing with projections no reliable geospatial data can be used.

COMMERCIAL STATIONS (filtered to show more detail)
![Screenshot 1](https://github.com/seanhulseman/FM-Broadcast-Landscape/blob/main/images/commercial_fm_stations.png?raw=true)
EDUCATIONAL STATIONS (filtered to show more detail)
![Screenshot 2](https://github.com/seanhulseman/FM-Broadcast-Landscape/blob/main/images/educational_fm_stations.png?raw=true)
[Add any relevant screenshots from the images folder]

## License
Created: 2024 Sean Hulseman

## Contact
* Email me with any questions: seanhulseman@gmail.com
* You can visit [this website](https://seanhulseman.github.io/) to find some of my work 
* View my LinkedIn [here](https://www.linkedin.com/in/seanhulseman/).


