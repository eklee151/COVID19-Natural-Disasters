# COVID19-Natural-Disasters
***

### Executive Summary
Fires can occur for many reasons. Some are caused naturally (think lighting striking a tree) and others are man-made (accidental or intentional). The year of 2020 has been unprecedented in the amount of destruction caused by fires across the country, all spurred by heat waves in some place, tropical storms in others, and even debris burning ((Source)[https://en.wikipedia.org/wiki/2020_California_wildfires; https://www.insurancejournal.com/news/southcentral/2020/08/17/579347.htm#:~:text=So%20far%20in%202020%2C%20902,a%20total%20of%20171%2C204%20acres]). It is important to note that not all fires are bad, some ecosystems depend on them and people use it in agriculture. Although not all fires that occur are detrimental, there are really important reasons why we should be actively tracking them. It helps us locate volcanoes, gas flares and the sources of air pollution caused by smoke ((Source)[https://earthdata.nasa.gov/earth-observation-data/near-real-time/hazards-and-disasters/fires]). 

The Coronavirus pandemic has plagued the world in the year 2020, and has been particularly deadly in the United States where, at the time this project was completed, total confirmed cases have just passed 9 Million, while deaths are at about 230,000. We began our exploratory data analysis by graphing cumulative confirmed for each state and comparing them to eachother, we then chose the top three states with the most total confirmed cases and mapped the top 10 counties in each state to observe the severity of infection rates at more granular level.

We then combined the information we had on the spread of the virus with the information we had about fires and heat anomalies to create an interactive map. The heatmap layer shows precise geographical locations of fires and heat anomalies in the United States from February to October 2020, and an additional chloroplet layer illustrates daily confirmed cases in each State for the same range of dates.

<br>

### Problem Statement
Can we create a web-based application that maps fires/heat anomalies as well as COVID-19 infection rates in the US? Is it possible to showcase a relationship between fire occurrences and COVID-19 infection rates?

<br>

### Hypothesis
We hypothesized that that people would be more likely to stay at home/indoors in areas with fires, thereby decreasing the likelihood of contracting COVID-19. 

<br>

### Contents:


### Data
This data set was provided by LANCE FIRMS operated by NASA ESDIS with funding provided by NASA Headquarters and can be found [here]( https://firms2.modaps.eosdis.nasa.gov/download/)
 - Covered the dates of 1/1/2020 – 10/23/2020
 - 41,709 fire occurrences for the continental US (including the District of Columbia), Alaska and Hawaii
 
COVID-19 statewide incidence numbers inputted into folium can be found [here](https://covidcast.cmu.edu/?sensor=doctor-visits-smoothed_adj_cli&level=county&date=20201018&signalType=value&encoding=color&mode=overview&region=42003)

COVID-19 data used in EDA graphs can be found [here](https://raw.githubusercontent.com/kevinrenois/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_US.csv)

### Data Dictionaries
|Feature| Type| Description|
|---|---|---|
|**latitude**|numeric| latitude|
|**longitude**|numeric| longitude|
|**brightness**|numeric| channel 21/22 brightness temperature of the fire pixel ( in Kelvin)|
|**scan**|numeric| along scan pixel size|
|**track**|numeric| along scan pixel size|
|**acq_date**|date| date of MODIS acquisition|
|**acq_time**|numeric| time of /overpass of the satellite (in UTC)|
|**satellite**|categorical| Aqua vs. Terra satellite|
|**instrument**|categorical| Imaging instrument|
|**confidence**|numeric| score representing how confident the software is that a fire is present in the location|
|**version**|categorical| collection and source|
|**bright_t31**|numeric| channel 31 brightness temp of the fire pixel (in Kelvin)|
|**frp**|numeric| fire radiative power (in megawatts)|
|**daynight**|categorical| inferred hot spot type|
|**type**|categorical|url D = daytime fire, N = nighttime fire|

<br>

## COVIDcast Statewide Incidence Data
|Feature| Type| Description|
|---|---|---|
|**geo_value**|string| state|
|**signal**|string|name of signal derived from upstream data|
|**time_value**|string| month, day, year |
|**issue**|list of time values|time unit when the signal data were published|
|**lag**|integer|time between when the underlying events happened and when the data were published|
|**geo_type**|string|spacial resolution of the signal(e.g. state|
|**data_source**|string|name of upstream data source|

<br>

### Conclusions/ Recommendations

