# The Radio Landscape Project

## Introduction

The Radio Landscape Project originated from a personal curiosity during a road trip in August 2022. As I traversed through various regions, I couldn't help but notice the stark differences in radio offerings within just a few dozen miles. This project aims to explore the multifaceted aspects of the radio landscape, including the number of stations available, the diversity of music genres, the types of programming offered (such as news, sports talk, political discourse, religious content), and the regional variations in listenership habits. By delving into these nuances, we hope to uncover insights into political, sociological, business, educational, and religious dynamics across different regions.

## Objectives and Questions

- Investigate the regional variations in radio programming and listenership habits.
- Analyze the impact of radio station diversity on societal and cultural dynamics.
- Explore correlations between radio preferences and sociopolitical factors.
- Examine the implications of commercial vs. educational radio stations on communities.

## Data Collection

The project utilizes data obtained from the FCC FM Radio Query tool, which provides detailed information about radio stations across the United States. After retrieving the raw data, efforts were made to clean and preprocess it, including addressing encoding issues and labeling stations as commercial or educational.

## Dataset Availability

The 'FM_stations_labeled.csv' dataset created from the FCC FM Radio Query is available for public use. Feel free to explore and analyze this dataset, and don't hesitate to contribute to the project by sharing your findings or suggestions.

## Project Status

As of January 30th, 2024, the project is still in its early stages and is a work in progress. Updates will be made to this README.md and the project repository as more progress is achieved.


## Features
* **jupyter notebook 1** - Obtaining the data, label edu and commercial, N/S,D,M,S --->(latitude) and W/E,D,M,S --->(longtitude) decimal form for geodatframe later - save the master csv - NO DROPPING HERE What else can I do with the data?
* **jupyter notebook 2** - EDA and Cleaning (NULL ISLAND), UNITS! For the different services - research more on what those mean. Do they need different considerations than others? DA, NA?, FM Status
* **Jupyter notebook 3 (USE GOOGLE COLAB)** - Geopandas - geospatial mapping, projections, energy flux(research the physics), kde density plots, 
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
MIT License

Copyright (c) [year] [author]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Contact
You can visit my website showcases some of my projects [here](https://seanhulseman.github.io/), and my LinkedIn [here](https://www.linkedin.com/in/seanhulseman/)