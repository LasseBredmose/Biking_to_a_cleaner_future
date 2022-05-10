---
title: Biking to a cleaner future
layout: single
---

# Good, better, Copenhagen 
At least 50% percent should bike to school or work, better parking facilities for bicycles at stations, 30-40 km of additional tracks and lanes. Such are some of the goals stated in the initiative *Good, Better, Best - The City of Copenhagen’s Bicycle Strategy 2011-2025* introduced by the city council of Copenhagen in 2011. This was created as a part of making Copenhagen a carbon neutral city in the year of 2025 [1]. With 2025 coming closer, we take a deep dive to investigate just how the initiaves have influenced the copenhagernes' bicycling habits. We will look into whether changes at a 10-year period from 2009 to 2018 can be spotted, and if vehicles still dominate the roads across Copenhagen. Finally we include weather conditions to analyze their influences on our daily transportation patterns.

# Data

<div>
<iframe src="/html/map_points.html"
	sandbox="allow-same-origin allow-scripts"
	width="60%"
	height="425"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	align="left"
	style="margin-right: 0.5em; margin-top: 0.4em; margin-bottom: 1em;">

</iframe>
</div>

To conduct our analysis, we need some data. Thus the data used is a preprocessed [*traffic dataset from OpenData*](https://www.opendata.dk/city-of-copenhagen/trafiktal), originally collected by the Copenhagen Municipality. The data has further been combined with the original raw dataset to gain further information and limited to a 10-year period of 2009 to 2018. The data is obtained by people (our so-called *counters*) who have stood at various locations in Copenhagen to count the number of passing bikes and cars. Most of the *counters* have been placed in central Copenhagen, Vesterbro and Nørrebro, along with some of the main roads. This can be seen on the map to the left, for which the reader is encouraged to explore. There are even a few *counters* in Frederiksberg, although the district not being within the municipality, but no *counters* in Nordhavn.

## Inspection throughout years
Firstly, let us look at the entire time period and the levels for bikes and cars for each year. The number of observations for our two modes of transport is steady throughout the years, although a drop is seen for the year of 2017. It might be tempting to jump the conclusion that there must have been less bikes and less cars within this year, but it is important to keep in mind that we are dealing with count data! So there could be other reasons for this dip. Let us inspect whether this is the case by **hovering** over the bars in the visualization.
<iframe src="/html/num_obs_by_year.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	align="center"
	height="420"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>
We see that the fraction of bikes and cars stays somewhat constant for all years, but there are less counters for the year of 2017, which could have caused the drop. We would expect that the fewer counters we have, the less observations there will be. However, by further inspection, the number of counters might not be the entire reason for this phenomenon. The drop in counters from 2014 to 2015, for example, is 60 - the exact same as the drop in counters from 2015 to 2017. However, the gap in the number of observations is much larger from 2015 to 2017, than between 2014 and 2015. Therefore, we could imagine that other factors could also have contributed to the drop.

## Inspection throughout months
Nextly, we can take a look at the monthly time period, accumulated throughout all years. In a provided *counting guide* , we observe that the frequent counting months are May, June, August, September, and October [2]. Looking at the data, we observe a relatively high amount of observations in April. By **hovering** over the bar, we are informed that the month of April is one of the months with most counters, despite not being featured as an official month from the guide. Unfortunately, we can only speculate on why this is the case. However, as they do special countings ordered by external entities, such as the *University of Aarhus* or *Vejdirektoratet*, more pressing matters might have forced them to count outside the regular schedule. 
<iframe src="/html/num_obs_by_month.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="420"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>
In August, we notice a small amount of counters along with a small amount of observations, which also diverges from the guide, stating that August is an active counting month. However, a deeper look into the guide tells us that August, along with June, are active months for counting pedestrians. Thus, it can be a reason why we see observations for these months, as some counters might have included bikes and cars in their countings.

# Daily patterns
It is difficult to obtain sufficient information of patterns throughout the years and months. Instead, let us look at the development in activity from 7 to 19. For both bikes and cars, the peaks are in the morning and afternoon, which fits with when most people need to go to work, school or other daily obligations and return home. For gaining a simple overview, it is also possible to only look at cars or bikes, by **toggling** either cars or bikes off in the plot. 
<iframe src="/html/num_obs_by_hour.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="420"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>

It is worth noticing that there is a difference in the ratios between bikes and cars in the morning. From 7 to 8, the gap between the amount of cars and bikes is larger than from 9 to 10. This could be explained by how people with cars tend to have a longer commute e.g. having to get out of the city, or dropping off kids, thus having to leave their home earlier. With a car, traffic also plays a larger factor than with bikes. It would thus not be entirely surprising if there is a need for getting up earlier to avoid running into that.

## Spatial patterns
Knowing the daily development in activity in the entire city, a question arises about whether the same trend is seen across each counting spot. And if not, it would be interesting to inspect exactly which places that encounter a lot of changes in activity through the day.

### Bikes
We start by investigating the changes in activity for the bikes. In the video below, it is shown that there is constant activity around central Copenhagen throughout the entire day. Central Copenhagen, or *Indre by* is where we find many shopping opportunities, tourist attractions and workplaces. It is thus not surprising that this part will incur a lot of buzz with biking being a mode of transportation that makes it easy to get around to various attractions, cafés etc., even outside of rush hour.

By **playing** the video, it can be seen that during rush hour, both in the morning and late afternoon, the activity has more of a spread, no longer being as concentrated around the center. The spread is e.g. towards *Nørrebro*. This would be due to how people get to and off work and would have to ride their bikes throughout the various districts outside center.

<iframe src="/html/map_time_bike.html"
	id="left_frame"
	sandbox="allow-same-origin allow-scripts"
	width="95%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	style="margin-top: 1em; margin-bottom: 1em">
</iframe>

The reader is encouraged to use the **hover tool** to discover the aggregated total amount of bikes in Copenhagen. From here, we see that *Indre By* is the district with by far the most bikes throughout the entire time period also, fitting with how the activity level is always high here.

### Cars
For cars, it is a bit of a different story, although similar in some areas. *Indre By* remains the district that constantly has high levels of activity, but interestingly, there is a larger spread of cars throughout various other districts than with bikes. This is especially seen during the morning and afternoon, which follows closely with how people with cars would have longer commutes and thus having to pass the outer districts too.

<iframe src="/html/map_time_cars.html"
	id="right_frame"
	sandbox="allow-same-origin allow-scripts"
	width="95%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	style="margin-top: 1em; margin-bottom: 1em">
</iframe>

By **zooming in on the map**, it is seen that there is a clear impact on many of the main roads leading into and out of *Indre By* such as *Ågade*, *Åboulevard*, *Nørre Allé* and *Tuborgvej*. Also, high activity points can be found for roads leading out of the city, e.g. *Frederikssundsvej*, *Jyllingevej*, *Roskildevej*, *Hareskovvej* and *Strandvejen*, indicating that people with cars would have longer commutes. Thus riding a bike might not be a straight forward option, especially when considering the additional travel time and the unpredictable weather in Denmark.

# Impact of the weather

<div>
<iframe src="/html/map_weather.html"
	sandbox="allow-same-origin allow-scripts"
	width="70%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	align="right"
	style="margin-left: 0.5em; margin-top: 0.4em; margin-bottom: 1em;">

</iframe>
</div>

As mentioned earlier we have acquired data of the specific weather conditions for the days where the countings took place. The data is measured using three different weather stations, measuring precipitation, wind and/or temperature. The specific measurement type for each of the weather stations can be seen by **clicking** on the information markers on the map. In order to work further with the data, we have taken an average of the measurements for those days where multiple weather stations have collected the same measurement type.  
<br/>
<br/>
<br/>
<br/>
<br/>
In the graphs below we can see the measurements for the temperature, wind speed, and precipitation. Each data point is added as a dot on the graph, thus one can see which periods we have datapoints for.
For the temperature, we observe that the values always stay positive while frequently getting above 15 degrees. Looking at both the temperature and precipitation, we observe that there are very few days with high precipitation, which implies that most of the counting has taken place on sunny days. The wind speed does not seem to have an impact in the selection of days, where the counters have been out, as it fluctuates between 2 and 8 m/s. The reader is incurred to **click and drag** to explore weather data for the whole period. 


<iframe src="/html/temp_wind_precip_development.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="630"
	scrolling="no"
	seamless="seamless"
	frameborder="1"
	style="margin-bottom: 1em;">
</iframe>

The impact of the weather conditions has been investigated in the following figures. Here, the average number of observations for bikes and cars are shown within different intervals for temperature, wind speed and precipitation. 

<iframe src="/html/temp_wind_precip_bikescars.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="380"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>

Considering the temperature, we see a trend for the average number of bikes. As expected, the higher the temperature, the more bikes are seen in the streets. This trend, however, drops for temperatures higher than 20 degrees. Looking at the average number of cars, we see (almost) the opposite trend. The average number of cars decreases as the temperature increases - again, until the temperature is higher than 20 degrees. Such relationship can be questioned as it might be caused by lack of data in the Summer period where the temperature is usually at its highest. 
In regard to the wind speed, we notice a larger average number of bikes being counted when the wind speed is less than 2 m/s. From this, it drops and becomes more steady throughout the remaining wind speed intervals. Thus, it seems like some people brave the weather during these windy days. However, it is noticed that when the wind speed is high, there is in average also more cars in the streets of Copenhagen. This does not come as a surprise since you will not be affected by the wind when sitting in a car.
When it comes to precipitation, the traffic data did unfortunately (almost) not include days with precipitation. Thus, the figure does not include much information about the patterns in bikes or cars for days with precipitation.

</br>

Having an overview of how weather might impact the patterns in terms of modes of transportation, we have tried to conduct machine learning to predict the amount of cars and bikes given the weather conditions. The models that were used were various linear regression models and a random forest regressor. If interested, we encourage visiting our [explainer notebook](https://deepnote.com/@maria-fogh/SocialDataProject2022-61ec0a5b-e327-402f-95c1-91c4aeb91c25) for a comprehensive review of these.

# Final Words
From our analysis, we have looked into our dataset, which contains measurements with the amount of bikes and cars in Copenhagen over a 10-year period. Here, we discovered that cars still remains the dominant mode of transport on the streets of Copenhagen despite the initiatives from the Copenhagen Municipality. From inspecting the dataset in terms of the years and the months, we found inconsistencies, such as how it is not the same number of counters that have participated each year, leading to a variation in terms of measurements taken. Also, the countings have only been conducted in late Spring and early Fall, causing biases in our dataset. This would have been resolved by finding automatically counted data at the same locations each year. From spatial and temporal patterns throughout the day, we observed how people get into and out of the city in accordance to work patterns, but still differently for cars and bikes. We also employed weather data to investigate the impact of different weather conditions. Here, it was also seen that the biases come into play, as most of our measurements are taken on sunny and warm days (without precipitation).


# References
* [1] Baykal, Ayfer(2011). "Good, Better, Best - The City of Copenhagen’s Bicycle Strategy 2011-2025", The city of Copenhagen, available [HERE](https://web.archive.org/web/20120906180553/http://www.kk.dk/sitecore/content/Subsites/CityOfCopenhagen/SubsiteFrontpage/LivingInCopenhagen/CityAndTraffic/CityOfCyclists/~/media/A6581E08C2EF4275BD3CA1DB951215C3.ashx)
* [2] Henrichsen, Åse Boss and Spliid, Lone(2020). "Sådan udfører vi trafiktællinger i Københavns kommune". Municipality of Copenhagen: Københavns Teknik- og Miljøforvaltning. Available [HERE](https://github.com/LasseBredmose/social_data_2022_project/blob/main/Trafiktællevejledning.pdf)
