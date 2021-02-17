---
layout: default
title: Add POPULATION Data
nav_order: 1
parent: Analyzing Data
---

## ADD POPULATION DATA

Just as we did in the first exercise, we can search for layers in the Living Atlas that make our map more meaningful.
Census data provides population and dwelling data by dissemination area that is provided by [Statistics Canada](https://open.canada.ca/data/en/dataset/3cf36302-1060-444e-988a-d97b6db5ad24) but symbolized and made available through the Living Atlas, making it more accessible.

[Dissemination areas](https://www12.statcan.gc.ca/census-recensement/2011/ref/dict/geo021-eng.cfm) (DAs) are the smallest geographic area used in the Canadian Census data and represent 400 to 700 individuals or approximately 250 households.

Adding data on population and dwelling counts to our map helps contextualize the locations of Vancouver's homeless shelters.

To Do
{: .label .label-green }
From your web map, click the **Add** dropdown arrow and select **Browse Living Atlas Layers**.

*1*{: .circle .circle-blue} In the search box, type **census canada dissemination** and click the plus sign next to **Canadian Population & Dwelling Counts by Dissemination Area, 2016** to add it to the map.

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


