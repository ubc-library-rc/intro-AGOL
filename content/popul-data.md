---
layout: default
title: Add Population Data
nav_order: 1
parent: Analyzing Data
---

## ADD POPULATION DATA

Just as we did in the first exercise, we can search for layers in ArcGIS Online that make our map more meaningful.

Census data from [Statistics Canada](https://open.canada.ca/data/en/dataset/3cf36302-1060-444e-988a-d97b6db5ad240) is normally a great place to find population information, but it's also usually distributed by area, whether Census subdivisions or dissemination areas. Two layers of polygons stacked on top of one another are difficult to view.

[Agriculture and Agri-Food Canada](https://www.agr.gc.ca/eng/agriculture-and-agri-food-canada/?id=1395690825741) has a robust [ArcGIS Online presence](http://bit.ly/16o91lM), and they also happen to publish population data in a way more useful for our purposes. They produce the [Canadian Ecumene Database](https://open.canada.ca/data/en/dataset/3f599fcb-8d77-4dbb-8b1e-d3f27f932a4b) representing populated places. Ecumene is a word meaning "inhabited lands."

Let's see if we can find and add this dataset to our web map.

To Do
{: .label .label-green }
From your web map, click the **Add** dropdown arrow and select **Search for Layers**. From the dropdown arrow, make sure **ArcGIS Online** is selected.

*1*{: .circle .circle-blue} In the search box, type **canada population ecumene** and click the plus sign next to two layers for comparison. **The Canadian Ecumene (CanEcumene) 2.0 GIS Database** and **Populated Places - Canadian Ecumene**.

The latter layer is produced by Esri Canada using data from The Canadian Ecumene GIS Database.

This data layer uses [chloropleth](http://wiki.gis.com/wiki/index.php/Choropleth_map) symbology, in which areas are shaded or patterned proportionally to the value of a variable measured for each area.

- The variable is usually quantitative
- A color is associated with an attribute value
- It's a method for showing how a measurement varies across a geographic area

You can read more about and see examples of chloropleth [maps](https://arcg.is/15Xffe).

Although this Census data provides context, it also overwhelms the homeless shelter location data, which we want to be more prominent.

*2*{: .circle .circle-blue} First hover over the left and then drag the Census layer below the homeless shelter location data.

*3*{: .circle .circle-blue} Next click on the layer and then on the ellipsis and select **Transparency** from the dropdown.
Use the slider to position it somewhere between 50% and 75% and save your map.

Let's see if we can find additional data through the Living Atlas that might help make our map more meaningful, such as Census data on poverty or homelessness.

*4*{: .circle .circle-blue} Type **census poverty** into the search bar under **Add Data>Browse Living Atlas Layers**

There are a number of layers that come up, but unfortunately all of these represent data from the U.S. Census, which reveals a weakness of the Living Atlas in that it is U.S.-centric.

It also underscores how useful the Living Atlas is when data we want is available because searching for the right data in the correct GIS format can be time consuming and frustrating.

*5*{: .circle .circle-blue} Try searching for **census poverty Canada** or **census homeless Canada** to see if you can find anything related to Canada.

Nothing comes up, and finding GIS data for metro Vancouver on the homeless populations, income, and poverty is very difficult to find. Instead of finding additional data for our map, we'll use other information to add to a [story map](https://storymaps.arcgis.com/stories) about domestic violence, homeless shelters that allow pets and the relationship of these to the capacity of domestic violence victims to leave their abusers.


