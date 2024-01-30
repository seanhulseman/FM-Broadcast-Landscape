# FM Broadcast Landscape

## Introduction
The radio landscape is an idea I came up with on a road in august 2022. I wanted to understand, as I drove away from familiar cities, how the radio options were so vastly different over a few dozen miles of highway. The number of stations my radio picks up, the variety and genres of music available, the type of programming(News, sportstalk, talk, overtly political talk, religious, etc.) The number number of different channels used by the same station in any location(think boosters and translators*).

The FCC FM Radio Query was used to collect the data and label commercial vs educational stations. There are many directions one can take a project based on this data and I encourage anyone to feel free to use the 'FM_stations_labeled.csv' I created in the first jupytper notebook to explore! 

As of 1/30 the project is no where near complete. A lot of this is stream of conciousness and will need to be cleaned up and updated as more progress is made!

## Features
* **jupyter notebook 1** - Obtaining the data, label edu and commercial, N/S,D,M,S --->(latitude) and W/E,D,M,S --->(longtitude) decimal form for geodatframe later - save the master csv - NO DROPPING HERE What else can I do with the data?
* **jupyter notebook 2** - EDA and Cleaning (NULL ISLAND), UNITS! For the different services - research more on what those mean. Do they need different considerations than others? DA, NA?, FM Status
* **Jupyter notebook 3 (USE GOOGLE COLAB)** - Geopandas - geospatial mapping, projections, energy flux(research the physics), kde density plots, 
* **App** - Interacting with the stations - search a location, hear a station? display stations? Listen to a station? - big owners (IHM ex) may have ways to listen to many stations. the process to find those can be automated????
* **Jupyter Notebook 4** - Modeling - Predict commercial or educational. For census cities, what is the general diversity in radio landscape between those two measures. Can I group the stations further using NLP by company owner? Station description scraped? EDU stations - [College, Religious?, News/Talk?, Music?, grab bag? ,.... ]. Commercial [ genres/music?, major owners and everybody else? News/Talk?,]


## Installation
Geopandas and other geospatial software are a pain to install locally but Google Colab seems to work well enough! Most, if not all, geodataframe work will be done in Google Colab notebooks usable on any device.

## Usage
Make a copy of Colab Notebooks

## Preliminary images
This is a proof showing that my DMS ---> Decimal conversion worked. Without properly dealing with projections no reliable geospatial data can be used. 

COMMERCIAL STATIONS (filtered to show more detail)
![Screenshot 1](images\commercial_fm_stations.png)
EDUCATIONAL STATIONS (filtered to show more detail)
![Screenshot 2](images\educational_fm_stations.png)
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