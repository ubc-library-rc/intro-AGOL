---
layout: default
title: Add Your Own Data
nav_order: 5
has_children: true
---

## ADD YOUR OWN DATA

In ArcGIS Online, you can add data from the Living Atlas, curated by Esri, from web services produced by other agencies, or you can add your own data.

There are multiple data formats that can be added to an AGOL web map. 

 - [shapefile](https://desktop.arcgis.com/en/arcmap/latest/manage-data/shapefiles/what-is-a-shapefile.htm) - to be added to the map, the different components of the shapefile must be compressed into a ZIP archive
 - CSV or TXT files with optional address, place or coordinate locations (comma, semi-colon or tab delimited)
 - GPX (GPS Exchange Format)
 - [GeoJSON](https://geojson.org/) (open standard format for simple geographical features)
 
We want to zoom in on the map and explore the pandemic from a more localized perspective. Let's try and better understand COVID-19 data in Canada. 

In additon to Statistics Canada, there are some other places we can find data about COVID-19 in Canada. Some provide data for download, and some sites proivde visualizations or maps with the data available. Below is a list of just some of the COVID-19 data resources.

[Esri COVID-19 Open Data](https://resources-covid19canada.hub.arcgis.com/pages/open-data)

[University of Toronto Libraries COVID-19 Data Resources](https://mdl.library.utoronto.ca/covid-19/resources)

[Flatten](https://www.flatten.ca/)

[COVID-19 in Canada](https://art-bd.shinyapps.io/covid19canada/)

[COVID-19 Canada Open Data Working Group](https://opencovid.ca/)

[Canada COVID-19 interactive growth rate explorer](https://mountainmath.ca/shiny/canada_covid-19/?_inputs_&level=%22province%22&metric=%22Confirmed%22&province=%2201%22&start_cutoff=100)

Because we're working in ArcGIS Online, let's take a look at Esri's data hub for COVID-19 data in Canada. 

ADDED TIMESERIES CASE DATA - NEXT STEPS SYMBOLIZE AND ADD INSTRUCTIONS FOR THIS; CITE SOURCE

On June 16, 2020, the news site [*The Conversation*](https://theconversation.com/ca) published an [article](https://theconversation.com/people-in-abusive-relationships-face-many-barriers-to-leaving-pets-should-not-be-one-139540?utm_medium=email&utm_campaign=Latest%20from%20The%20Conversation%20for%20June%2017%202020&utm_content=Latest%20from%20The%20Conversation%20for%20June%2017%202020+CID_e7708191b09d4919198c361914f475ff&utm_source=campaign_monitor_ca&utm_term=pets%20should%20not%20be%20one) about one of the barriers preventing people from leaving abusive relationships: pets. The article states that some people may be more reluctant to leave an abusive relationship if they are unable to take their pet with them or are worried for its safety if they leave it home with the abuser.

Geographic data on intimate partner violence (IPV) shelters is difficult to find because making their locations known to the public would also make their locations knowable to abusers. 

[Evidence](https://www.acf.hhs.gov/fysb/resource/dv-homelessness-stats-2016) in the United States suggests that there is lack of sufficient housing in IPV shelters and also that for some women, homelessness intersects with domestic violence.

Assuming that homeless shelters are one place domestic abuse survivors sometimes access for safe harbor, let's see if we can find data related to homeless shelters in Vancouver in order to find out which homeless shelters accomodate pets.

The City of Vancouver maintains the [Open Data Portal](https://opendata.vancouver.ca/pages/home/) where users can download data, view data in a map, or build a chart, among other functionalities.

You should have downloaded this data in preparation for our workshop, but in case you didn't, you can [download](https://opendata.vancouver.ca/explore/dataset/homeless-shelter-locations/download/?format=geojson&timezone=America/Los_Angeles&lang=en) it now. 

In the next section, we'll add this GeoJSON file of [homeless shelter locations](https://opendata.vancouver.ca/explore/dataset/homeless-shelter-locations/export/) to our AGOL map.

