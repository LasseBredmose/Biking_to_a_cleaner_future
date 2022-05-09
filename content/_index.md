---
title: Biking to a cleaner future
layout: single
---

# Good, better, Copenhagen 
Every other should bike to school or work, better bicycling parking facilities at stations, 30-40km additional tracks and lanes. Such are some of the initiatives stated in the initiative *Good, Better, Best - The City of Copenhagen’s Bicycle Strategy 2011-2025* introduced by the city council of Copenhagen in *2011*. Created as a part of making Copenhagen a carbon neutral city in the year of *2025*. With *2025* coming closer we take a deep dive into see just how the initiave have influence the copenhagernes bicyckling habbits, if one can spot changes looking at a 10-year period from *2009* to *2018*, and if vehicles still dominate the roads across Copenhagen.
Finally we take a *hard* look on external factors, such as weather and temperature in order to anaylse and perhabs predict influences corralated with up's and down's in the habits of taking the car or bike. 

**Include quick summation of what we will talk about?**

# Data

<div>
<iframe src="/html/map_points.html"
	sandbox="allow-same-origin allow-scripts"
	width="60%"
	height="450"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	align="left"
	style="margin-right: 0.5em; margin-top: 1em; margin-bottom: 1em;">
</iframe>
</div>

To conduct our analysis, we need some data. Thus the data used is a preprocessed [traffic data set from OpenData](https://www.opendata.dk/city-of-copenhagen/trafiktal), originally collected by the Copenhagen Municipality. The data has further been combined with the original raw dataset to gain further information and limited to a 10-year period of 2009 to 2018. The data is obtained by people (our so-called *counters*) who have stood at various locations in Copenhagen to count the number of passing bikes or cars. Most of the *counters* have been placed in central Copenhagen, Vesterbro and Nørrebro, along with some of the main roads. This can be seen on the map to the left, for which the reader is encouraged to explore. There are even a few *counters* in Frederiksberg, although the district not being within the municipality and no *counters* in Nordhavn.

## Inspection throughout years
Firstly, let us look at the entire time period and the levels for bikes and cars for each year. The number of observations for our two modes of transport is steady throughout all years, although a drop is seen for the year of 2017. It might be tempting to jump the conclusion that there must have been less bikes and less cars within this year, but it is important to keep in mind that we are dealing with count data! So there could be other reasons for this dip. Let us inspect whether this is the case by **hovering** over the bars in the visualization.
<iframe src="/html/num_obs_by_year.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	align="center"
	height="420"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>
We see that the fraction of bikes and cars stays somewhat constant for all years, but there are less counters for the year of 2017, which could have caused the drop. We would expect that the fewer counters you have, the less observations there will be. However, by further inspection, the number of counters might not be the entire reason for this phenomenon. The drop in counters from 2014 to 2015, for example, is 60 - the exact same as the drop in counters from 2015 to 2017. But the gap in the number of observations is much larger from 2015 to 2017, than between 2014 and 2015. Therefore, we could imagine that external factors could also have contributed to the drop.

## Inspection throughout months
<iframe src="/html/num_obs_by_month.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>

# Temporal Patterns
<iframe src="/html/num_obs_by_hour.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>

# Spatial Patterns
## Bikes
<iframe src="/html/map_time_bike.html"
	id="left_frame"
	sandbox="allow-same-origin allow-scripts"
	width="95%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	style="margin: 0.2em;">
</iframe>
Hej hvordan har du det

## Cars
<iframe src="/html/map_time_cars.html"
	id="right_frame"
	sandbox="allow-same-origin allow-scripts"
	width="95%"
	height="500"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	style="margin: 0.2em;">
</iframe>

# Impact of the weather
Weather is always nice

# ML
mldkjhfng
nnmkdjnb

ndlkfnb


dnlkbnd  

dlkgndkb  

dlkgn kdn

 dkfg dlk
 
  dkgn dn 'dg 
  dogj
   djg
   d jg
   dgjk d
   kg 
   d 
   
   
   doljgdælkg

# Conclusion


# References
## Links and websites
* [Wiki_cyckling](https://en.wikipedia.org/wiki/Cycling_in_Copenhagen#Infrastructure)
* [Cyckling, better and best](https://web.archive.org/web/20120906180553/http://www.kk.dk/sitecore/content/Subsites/CityOfCopenhagen/SubsiteFrontpage/LivingInCopenhagen/CityAndTraffic/CityOfCyclists/~/media/A6581E08C2EF4275BD3CA1DB951215C3.ashx)
* [Urban cycling in cph](https://urbandevelopmentcph.kk.dk/node/14)

## [Explainer Notebook](explainer-notebook.html)

** The website **
* Introduction/Motivation(short)
* Tælledata, map hvor vi har talt henne. Ref til åsepiges pdf. 
* Udviklingen gennem årerne. Sker ikke så meget, interessant i 2017. nok bare talt mindre? 


