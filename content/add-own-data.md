---
layout: default
title: Add Your Own Data
nav_order: 5
has_children: true
---

## ADD YOUR OWN DATA

In ArcGIS Online, you can add data from the Living Atlas, curated by Esri, from web services produced by agencies such as the City of Vancouver, or you can add your own data.

There are multiple data formats that can be added to an AGOL web map. 

 - [shapefile](https://desktop.arcgis.com/en/arcmap/latest/manage-data/shapefiles/what-is-a-shapefile.htm) - to be added to the map, the different components of the shapefile must be compressed into a ZIP archive
 - CSV or TXT files with optional address, place or coordinate locations (comma, semi-colon or tab delimited)
 - GPX (GPS Exchange Format)
 - [GeoJSON](https://geojson.org/) (open standard format for simple geographical features)
 
Exploring spatial components of data can help us answer questions about the world and our environment.

On June 16, 2020, the news site [*The Conversation*](https://theconversation.com/ca) published an [article](https://theconversation.com/people-in-abusive-relationships-face-many-barriers-to-leaving-pets-should-not-be-one-139540?utm_medium=email&utm_campaign=Latest%20from%20The%20Conversation%20for%20June%2017%202020&utm_content=Latest%20from%20The%20Conversation%20for%20June%2017%202020+CID_e7708191b09d4919198c361914f475ff&utm_source=campaign_monitor_ca&utm_term=pets%20should%20not%20be%20one) about one of the barriers preventing people from leaving abusive relationships: pets. The article states that some people may be more reluctant to leave an abusive relationship if they are unable to take their pet with them or are worried for its safety if they leave it home with the abuser.

Geographic data on intimate partner violence (IPV) shelters is difficult to find because making their locations known to the public would also make their locations knowable to abusers. 

[Evidence](https://www.acf.hhs.gov/fysb/resource/dv-homelessness-stats-2016) in the United States suggests that there is lack of sufficient housing in IPV shelters and also that for some women, homelessness intersects with domestic violence.

Assuming that homeless shelters are one place domestic abuse survivors sometimes access for safe harbor, let's see if we can find data related to homeless shelters in Vancouver in order to find out which homeless shelters accomodate pets.

The City of Vancouver maintains the [Open Data Portal](https://opendata.vancouver.ca/pages/home/) where users can download data, view data in a map, or build a chart, among other functionalities.

You should have downloaded this data in preparation for our workshop, but in case you didn't, you can [download](https://opendata.vancouver.ca/explore/dataset/homeless-shelter-locations/download/?format=geojson&timezone=America/Los_Angeles&lang=en) it now. 

In the next section, we'll add this GeoJSON file of [homeless shelter locations](https://opendata.vancouver.ca/explore/dataset/homeless-shelter-locations/export/) to our AGOL map.

