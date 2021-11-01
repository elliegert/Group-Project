# Research Proposal - Midterm Update
## Research Question
Our research question asks: What are the common characteristics of the built environment, specifically traffic corridors, that make them unsafe and/or deadly? This project will explore Los Angeles citywide data of street characteristics, land use, and traffic/transit characteristics (i.e. speed, road classification, etc.) to understand what the common characteristics are. Ultimately, identifying these common characteristics has the potential to impact planning, design, and policy decisions for a safer Los Angeles.
## Why 
This research question is important because, as a recent article from the Journal of Transport and Land Use states, “US pedestrian fatalities are at their highest level in nearly three decades and account for an increasing share of total traffic fatalities (16%)” (Schneider et. al., 2021). Not only is this alarming, but it’s something that can be ameliorated. This topic is important because it affects a large swath of the population: pedestrians, drivers, public transit users, and people who engage in active transportation. Additionally, this data can inform how cities prioritize where safety investments are made. For example, wealthier neighborhoods or those with political power are the areas where infrastructure improvements are often prioritized. However, by taking a proactive approach, this data can provide information as to where safety improvements should be made prior to the occurrence of severe or even deadly collisions. 
Building off of the work of Schneider et. al., titled United States fatal pedestrian crash hot spot locations and characteristics in the Journal of Transport and Land Use, our research predominantly focuses on how we can be more proactive in making safety improvements on our city streets. For example, if we know these particular conditions are dangerous, we can improve them before someone is injured. Crash data is also often unreported or incorrectly reported, particularly for vulnerable road users. People involved in crashes may not want to interact with police, insurance companies, or the state, and it is therefore likely that crashes are underreported in particular neighborhoods. Therefore, if we are only using crash data to prioritize safety improvements, as is common practice among city agencies, it is possible that we are missing locations that are equally as dangerous. 
## Spatial Scope
The spatial scope of this project will be at the city level, specifically the City of Los Angeles. We feel that this is the most useful scope because we are aiming to identify the common characteristics of unsafe traffic corridors within Los Angeles’ city limits. Additionally, the availability of citywide data makes this project feasible. Further, it makes sense to focus on one particular municipal level because of how agencies delineate infrastructure responsibility. This is research that would be of particular interest to LADOT, who is responsible only for LA City streets. Eventually, once common characteristics of unsafe streets and traffic corridors are identified for the city of Los Angeles, we could compare this to data at a larger scale to see if these common characteristics overlap with LA county-wide data. Further, the study by Schneider et. al.,  titled United States fatal pedestrian crash hot spot locations and characteristics looked at fatality data and physical characteristics nationally, but this scope will help us understand if the characteristics they identified hold true at the scale of Los Angeles, or if there are local conditions that make LA unique from other cities. 
## Data Sources
**Fatality and collision data**
  * _Los Angeles Collisions 2014 through 2019_
    * Description: This data set includes details about all of the road collisions from 2014 to 2019 on roads that are within the Los Angeles City jurisdiction, not including state highways. It includes many characteristics of each collision, including data like severity of injury, time of day, and what types of vehicles were involved. The data is available [here](https://geohub.lacity.org/datasets/ladot::los-angeles-collisions-2014through2019/about) as a CSV file, KML, Shapefile, and GeoJSON
    * Source: Los Angeles City GeoHub, from the The Statewide Integrated Traffic Records System (SWITRS) and prepared by RoadSafeGIS
 


**Physical characteristic data** 

_Data we are currently using:_
* Open Street Map data: building types, speed, highway type

_Other potential data sources for physical characteristics include:_
  * Regulatory signs
    * Description: This data includes traffic signs including speed limit, one way, no left turns, weight restrictions, and on the streets of Los Angeles. Sign descriptors, such as speed limit, no left turn, right turn only, etc. are included in this data set. 
    * Source:  Data can be found [here](https://geohub.lacity.org/datasets/regulatory-signs/explore?location=34.009903%2C-118.405989%2C13.00) from LA City Geohub, from Los Angeles Department of Transportation. 
  * [Traffic Counts](https://github.com/elliegert/Group-Project/blob/main/data/Traffic_Counts.zip)
  * Cross walks
  * Traffic counts
  * Street designations, which indicate for example, if the street is a small neighborhood street or a larger arterial road  
  * Land use, potentially from zoning map
  * Number of lanes
  * Speed limit
  * Medians
  * Intersection traffic control characteristics including traffic signals and signs

_Data we explored but aren't using_
* [LA City Census Data - Age](https://github.com/elliegert/Group-Project/blob/main/Group%20Assignments/Census%20Data%20Exploration/acs2019_5yr_B01001_14000US06037293306.geojson)
* [La City Census Data - Race](https://github.com/elliegert/Group-Project/blob/main/Group%20Assignments/Census%20Data%20Exploration/acs2019_5yr_B03002_14000US06037293306.geojson)

## Analysis and Scope
**Step 1** 

We will first analyze traffic fatalities data to identify hot spots that have had the highest number of traffic fatalities in Los Angeles. So far we have:
  * Mapped the locations of traffic fatalities, demonstrating the areas with the highest number of deaths.
  * Narrowed our scope to ~80 locations that have had 2 or more fatalities from 2014-2019.  

**Step 2**

We will analyze the physical characteristics of these locations, such as street width, speed limited, etc. We will analyze this data to determine what the most common characteristics of these hot spots are. So far we have explored: 
 * building types
 * street classifications
 * speed
Our analysis methods have included using counts to see which characteristics are most common, as well as plotting the characteristics on maps. 
Next steps would be to look at how these characteristics interact with eachother to understand if there are sets of common characteristics combinations. 

**Step 3** 

The next step, though we're not sure that we'll get to this within the scope of this quarter, would be to  look at Los Angeles as a whole to see if there are other locations that have these common characteristics, but that might not necessarily be fatality hot spots.  
* This map would show locations throughout LA that have the common characteristics we identified in the mentioned above. 

**Scope** 
There are a few scoping parameters we have started to define as we've explored the data. As we learn more about the available data sources and learn more about spatial analysis, we may narrow the scope further. 
* _Population_: We are looking at all traffic fatalities, including pedestrian, bicylists, and motorists. 
* _Physical boundaries for fatality “hotspots”_: We have been exploring what the physical boundaries of our “hotspot” locations are. We have set various parameters based on the characteristics. This is an area we need to continue to explore to see what makes sense for each characteristic. 
* _Time period for traffic fatalities_: We are looking at the traffic fatalities from 2014-2019.
* _Fatalities vs severe injuries_: The two common safety factors used by municipalities and The Statewide Integrated Traffic Records System (SWITRS) are fatalities and severe injuries. After exploring the crash data, just looking at fatalities over 5 years provides more than enough data points. We've narrowed out points down to look at where two or more fatalities have occured. 
## Conclusion 
From our research, the two main questions we expect to be able to answer are: 1. What are the common characteristics of the most dangerous roads in LA? 2. Are there locations in LA that have not yet had a high number of fatalities, but that have the common characteristics that make them very dangerous? 

Some further insights that we hope to be able to gain from our research can help us understand why there are locations with common characteristics that lack a high number of collisions or fatalities. For example, are these locations in neighborhoods where traffic crashes are more likely to be unreported due to neighborhood characteristics and demographics, do places with lower traffic counts just have fewer fatalities, are there other infrastructure investments in place that we did not analyze, etc.  

Ultimately, we hope to gain insight into where infrastructure investments and improvements can be made to prioritize safety on Los Angeles city streets before crashes happen. 


