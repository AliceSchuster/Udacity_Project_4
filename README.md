# Udacity_Project_1


## Motivation

The following project has been created as part of the [Udacity Data Science Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025).

Using the Munich Airbnb dataset, this project aims to answer the following three questions of interest:

##### 1. In which months are most Airbnb listings still available (total and by room type)?
##### 2. In which Munich areas (zip codes) are the best Airbnb listings (according to total rating)?
##### 3. Do cheaper listings have a lower rating compared to expensive listings? 


## Files

This project uses data from the [Munich Airbnb dataset](http://insideairbnb.com/get-the-data.html) (date compiled: 24th of December 2020)

The analysis includes detailed listings data (download: listings.csv.gz) as well as detailed calendar data for listings (download: calendar.csv.gz). The unzipped data are stored in the Data folder of this project. For plotting the data (see question 2), I've also downloaded the postcode maps (files plz-5stellig.shp, plz-5stellig.shx, plz-5stellig.dbf, and plz-5stellig.dbf) from [this website](https://www.suche-postleitzahl.org/plz-karte-erstellen).  

The [udacity_project_1.ipynb](udacity_project_1.ipynb)  - Jupyter notebook includes the full project analysis for all three questions.


## Installation

For this project, I've have used Python 3.7.3 and the following Python libraries:

- altair==4.1.0
- geopandas==0.8.2
- matplotlib==3.3.2
- numpy==1.19.4
- pandas==1.1.3
- seaborn==0.11.0
- shapely==1.6.4

## License
This project is released under the terms of the MIT license, and thus free for commercial and research use. See [LICENSE](LICENSE) for details.


## Results

##### 1. In which months are most Airbnb listings still available (total and by room type)?

February 2021 is the month with the highest availability rate, followed by January 2021 and March 2021. If we have a look at the availability rate by room type, we can see that entire home/apartments, private rooms and shared rooms also have the highest availability rate in January, February, and March 2021. Only hotel rooms are slightly more booked in January 2021 compared to the other months.

##### 2. In which Munich areas (zip codes) are the best Airbnb listings (according to total rating)?

Most of the highest rated areas (zip codes with a rating above 97: 81373, 80639, 81243, 80636, 80686) are placed in the West of Munich. The only exception is zip code 81545, which is placed in the South of Munich.

##### 3. Do cheaper listings have a lower rating compared to expensive listings? 

The results show that there is hardly no correlation between price and total review score. Many listings in the lower price range also have very high ratings. 

##### If you are interested to learn more, please visit [my blog article](https://alicewacker.medium.com/plan-to-stay-in-an-airbnb-in-munich-for-2021-take-a-look-and-get-some-insights-for-your-next-trip-a440cf67650).

