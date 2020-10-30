# COVID19-Natural-Disasters

### Executive Summary
Fires can occur for many reasons. Some are caused naturally (think lighting striking a tree) and others are man-made (accidental or intentional). The year of 2020 has been unprecedented in the amount of destruction caused by fires across the country, all spurred by heat waves in some place, tropical storms in others, and even debris burning ((Source)[https://en.wikipedia.org/wiki/2020_California_wildfires; https://www.insurancejournal.com/news/southcentral/2020/08/17/579347.htm#:~:text=So%20far%20in%202020%2C%20902,a%20total%20of%20171%2C204%20acres]). It is important to note that not all fires are bad, some ecosystems depend on them and people use it in agriculture. Although not all fires that occur are detrimental, there are really important reasons why we should be actively tracking them. It helps us locate volcanoes, gas flares and the sources of air pollution caused by smoke ((Source)[https://earthdata.nasa.gov/earth-observation-data/near-real-time/hazards-and-disasters/fires]). 

### Problem Statement
Can we create a web-based application that maps fires/heat anomalies as well as COVID-19 infection rates in the US? Is it possible to showcase a relationship between fire occurrences and COVID-19 infection rates?

### Hypothesis
We hypothesized that that people would be more likely to stay at home/indoors in areas with fires, thereby decreasing the likelihood of contracting COVID-19. 

### Contents:


### Data
This data set was provided by LANCE FIRMS operated by NASA ESDIS with funding provided by NASA Headquarters and can be found (here)[ https://firms2.modaps.eosdis.nasa.gov/download/]
 - Covered the dates of 1/1/2020 – 10/23/2020
 - 41,709 fire occurrences for the continental US (including the District of Columbia), Alaska and Hawaii
 
COVID-19 statewide incidence numbers inputted into folium can be found (here)[https://covidcast.cmu.edu/?sensor=doctor-visits-smoothed_adj_cli&level=county&date=20201018&signalType=value&encoding=color&mode=overview&region=42003]

COVID-19 data used in EDA graphs can be found here ()

### Data Dictionary
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

### Conclusions/ Recommendations

