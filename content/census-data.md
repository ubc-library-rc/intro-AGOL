---
layout: default
title: Add Census Data
nav_order: 2
parent: Add Your Own Data
---

## ADD CENSUS DATA

Just as we did in the first exercise, we can search for layers in the Living Atlas that make our map more meaningful.
Census data provides population and dwelling data by dissemination area that is provided by [Statistics Canada](https://open.canada.ca/data/en/dataset/3cf36302-1060-444e-988a-d97b6db5ad24) but symbolized and made available through the Living Atlas, making it more accessible.

[Dissemination areas](https://www12.statcan.gc.ca/census-recensement/2011/ref/dict/geo021-eng.cfm) (DAs) are the smallest geographic area used in the Canadian Census data and represent 400 to 700 individuals or approximately 250 households.

Adding data on population and dwelling counts to our map helps contextualize the locations of Vancouver's homeless shelters. Ideally, we would be able to find data specifically on homeless populations in Vancouver, but I was not able to find this.

To Do
{: .label .label-green }
From your web map, click the **Add** dropdown arrow and select **Browse Living Atlas Layers**.

*1*{: .circle .circle-blue} In the search box, type **census canada dissemination** and click the plus sign next to **Canadian Population & Dwelling Counts by Dissemination Area, 2016** to add it to the map.

This data layer uses [chloropleth](http://wiki.gis.com/wiki/index.php/Choropleth_map) symbology, in which areas are shaded or patterned proportionally to the value of a variable measured for each area.

- The variable is usually quantitative
- A color is associated with an attribute value
- It's a method for showing how a measurement varies across a geographic area

Although this Census data provides context, it also overwhelms the homeless shelter location data, which we want to be more prominent.

*2*{: .circle .circle-blue} First hover over the left and then drag the Census layer below the homeless shelter location data.

*3*{: .circle .circle-blue} Next click on the layer and then on the ellipsis and select **Transparency** from the dropdown.
Use the slider to position it somewhere between 50% and 75% and save your map.

As you can see, creating a web map using ArcGIS Online provides a number of preconfigured settings and tools while still giving the user the option to add data, change basemaps, customize symbology, filter the data, and configure popups, among other things.

You can read more about and see examples of chloropleth maps [here](https://arcg.is/15Xffe).

Using ArcGIS Online, you can also create [StoryMaps](https://storymaps.arcgis.com/stories) and more powerful, customized interactive maps using [WebApp Builder](https://www.esri.com/en-us/arcgis/products/web-appbuilder/overview).

In the next and final section of this workshop, we'll incorporate the web map we just created into a StoryMap.
