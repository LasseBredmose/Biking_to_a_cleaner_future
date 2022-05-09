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
	height="425"
	scrolling="no"
	seamless="seamless"
	frameborder="0"
	align="left"
	style="margin-right: 0.5em; margin-top: 0.4em; margin-bottom: 1em;">

</iframe>
</div>

To conduct our analysis, we need some data. Thus the data used is a preprocessed [*traffic data set from OpenData*](https://www.opendata.dk/city-of-copenhagen/trafiktal), originally collected by the Copenhagen Municipality. The data has further been combined with the original raw dataset to gain further information and limited to a 10-year period of 2009 to 2018. The data is obtained by people (our so-called *counters*) who have stood at various locations in Copenhagen to count the number of passing bikes or cars. Most of the *counters* have been placed in central Copenhagen, Vesterbro and Nørrebro, along with some of the main roads. This can be seen on the map to the left, for which the reader is encouraged to explore. There are even a few *counters* in Frederiksberg, although the district not being within the municipality and no *counters* in Nordhavn.

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
Next we can take a look at the monthly time period, accumulated throughout all of the years. From the *counting guide* **ref** we observe that the frequent counting months are May, Juni, August, September and October. Looking at the data we observe a relative high amount of observations in April. **Hovering** over the bar we are informed that infact the month of April is the 3. biggest 'counting month', despite not featuring as an official month from the guide. We can only guess as to why this is. However they do special countings orderer from external entities, such as the *University of Aarhus* or *Vejdirektoratet*, where more pressing matters might force them to count outside the regular schedule. 
<iframe src="/html/num_obs_by_month.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="420"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>
In August we notice a small amount of counters as well as a small amount of observations, which diverge from the guide once more, stating that August is a active counting month. However, a deeper look into the guide tells us that August, along with June, is a active month for counting pedestrians. Given at least one reason, why the amount of cars/bikes is so small. Adding that the small observations we have, simply could be miss-countings from the counting of pedestrians. 

# Daily patterns
As it is difficult to obtain sufficient information of patterns throughout years and months, let us look at the evolution throughout the day, from 7 to 19 as these are the limitations of the dataset. For both bikes and cars, the peaks are in the morning and in the afternoon, fitting with when most people need to go to work, school or other daily obligations and back home. 

<iframe src="/html/num_obs_by_hour.html"
	sandbox="allow-same-origin allow-scripts"
	width="100%"
	height="420"
	scrolling="no"
	seamless="seamless"
	frameborder="1">
</iframe>

It is worth noticing that there is a difference in the ratios between bikes and cars in the morning. From 7 to 8, the gap between the amount of cars and bikes is larger than from 9 to 10. This could be due to how people with cars tend to have a longer commute e.g. having to get out of the city, or they could have kids that need to be dropped off, thus having to wake up earlier. With a car, traffic also plays a larger factor than with bikes. It would thus not be entirely surprising if there is a need for getting up earlier to avoid running into that.

# Spatial patterns (KAN BLIVE LAVET TIL EN MINDRE SECTION)
Now that we know the daily evolution in the entire city, a question arises about whether the same trend is seen across the counting spots in the entire city. And if not, it would be interesting to inspect exactly which places that encounter a lot of changes in activity through the day.

## Bikes
We start by investigating the changes in activity for the bikes. In our video, it is shown that there is constant activity around central Copenhagen throughout the entire day. Central Copenhagen, or *Indre by* is where we find many shopping opportunities, tourist attractions and workplaces. It is thus not surprising that this part will incur a lot of buzz with biking being a mode of transportation that makes it easy to get around to various attractions, cafés etc - even outside of rush hour.

By **playing** the movie with our heatmap, it can be seen that during rush hour, both in the morning and late afternoon, the activity has more of a spread, no longer being as concentrated around the center. The spread is e.g. towards *Nørrebro*. This would be due to how people get to and off work and would have to ride their bikes throughout the various districts outside center.

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

The reader is encouraged to use the **hover tool** to discover the aggregated total amounts of bikes in Copenhagen of the entire data set. From here, we see that Indre By is the district with by far the most bikes throughout the entire time period also, fitting with how the activity level is always high here.

## Cars
For cars, it is a bit of a different story, although similar in some areas. *Indre by* remains the district that constantly have high levels of activity, but interestingly, there is a larger spread of cars throughout various other districts than with bikes! This is especially seen during the morning and afternoon, which follows closely with how people with cars would have to ride longer distances and thus having to pass the outer districts too.

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

By **zooming in on the map**, it is seen that there is a clear impact on many of the main roads leading into and out of *Indre by* such as *Ågade*, *Åboulevard*, *Nørre Allé* and *Tuborgvej*. Also, high activity points can be found for roads leading out of the city, e.g. *Frederikssundsvej*, *Jyllingevej*, *Roskildevej*, *Hareskovvej* and *Strandvejen*, indicating that those people with cars would have longer commutes. Thus riding a bike might not be as straight forward of an option, especially when considering the additional travel time and the unpredictable weather in Copenhagen.

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


# 4. Genre
* Which gerne of data story did you use?
> **magazine**The data is presented in a magasine with hints of slideshow. Giving us the opportunity to communicate our results in a nicely putted way, where the reader is not distracted by flashy icons or complicated buttons. Thus creating a narrative that is easy to follow, where the reader can create ones own view of that data. 

* Which tools did you use from each of the 3 categories of Visual Narrative (Figure 7 in Segal and Heer). Why?
> As to the visual narrative we have drawn inspiration from figure 7 given in Segal and Heer. 
>**establishing shot/splash screen** Here we structure the webpage with title, background image and quick overview of each sections in the top-bar. Given the reader a quick overview of what the article is about, and which areas he can expect to read about. 
>**Consistent visual platform and feature distinction** Further more we use the 'Consisten Visual Platform' and 'Feature Distinction' techniques, by keeping the same fond and colours throughtout the whole webpage. Keeping the colours in line with the background image, as well as having the same fond in **almost** all of our figures. The reader will then not have to get accustomed to new colours, or different plotting techniques. Thus he is able to focus on the narrative of our story. 

* Which tools did you use from each of the 3 categories of Narrative Structure (Figure 7 in Segal and Heer). Why?
> **Linear structure** The ordering of our story follows the linear structure, where the reader knows what lies ahead of him, and he can follow the red thread without other distractions. Giving the reader the opportunity for him to explore the webpage at his own pace. 
> **Hover Highlighting** Most of our figures include hovering details, given the reader the chance to explore the data for him/her-self, as well as accompyning the narrative, if the reader has a hard time understanding a point. The highlighting includes typically extra information, used as a background for our narrative, where we mention the possibly for the reader to hover over our data. 
> **Navigation buttons** From the topbar we have created navigational tools, such that the reader quickly can skim to the desired section. Thus allowing the reader to take a break from the page and quickly get accessed to the section he was at, or even sharing the article at a specific section. 
**Filtering??**
>**Explicit Instruction** The test is accompanied with instructions to when and where the reader can interact with the plots. Thus the reader is not required to *explore* the webpage him/her-self using unwanted time to figure out when and how he/she should interact with the figures.
>**Captions/headlines** The webpage make use of captions under each figure carefully explaining what is seen. Further more the use of headlines makes sure that the reader knows instantly what the figure is about. 
>**Introductory text** The webpage has an introdution, serving as a teaser for the reader. The introduction quickly convers what the webpage is about, capturing the reader and introduces why the project is important. 
>**Summary** Conclusion?
