---
layout: default
title: Change the Basemap
nav_order: 1
parent: Create a Web Map
---

## CHANGE THE BASEMAP

Whenever you open a new map in ArcGIS Online, it will open with a default **Topographic** basemap. It's easy to choose other basemaps depending on what kind of map you are trying to make, but all of these are in the [Web Mercator](https://en.wikipedia.org/wiki/Web_Mercator_projection) projection, which distorts size the closer you get to the North Pole. Take a look at your map again and notice how disproportionately large the Northern Territories are using the Topographic basemap.

A far better projection for Canada is the Lambert Conformal Conic, which you can see side-by-side in the image below with the Web Mercator projection.

<figure>
  <img src="../images/projection.png" alt="projection">
  <figcaption><a href="https://gis.blog.ryerson.ca/2020/11/03/how-to-lie-with-covid-19-maps/">The Web Mercator projection is often used for web mapping.</a> (c) <a href="https://gis.blog.ryerson.ca/about-the-author/">Claus Rinner,</a> <a href="https://creativecommons.org/licenses/by-nc/3.0/">CC BY-NC 3.0</a>.</figcaption>
</figure>

<p>&nbsp;</p>

 Let's try and find a basemap with the Lambert Conformal Conic projection by searching ArcGIS Online, since all of the basemaps in the gallery are Web Mercator.

To Do
{: .label .label-green }
From the left sidebar, click on **Add** and click on **Browse layers**.

*1*{: .circle .circle-blue} Select **ArcGIS Online** from the dropdown and then search for **Canada_Provincial_Boundaries_3347**. Add this to the map as the basemap by clicking on the layer and then **Use as basemap**.

Now any data we add to the map will reproject on the fly to this Lambert Conformal Conic projection.

*2*{: .circle .circle-blue} Click on the **Save and open>Save** text in the left sidebar which should have a blue dot next to it, prompting you to save your map.

You will need to give the map a title, add tags to make it discoverable later, and a summary.

*2*{: .circle .circle-blue} Call your map **COVID-19 Cases**

Add these tags: COVID-19, Canada

Summary: Map created as part of Intro to AGOL workshop.

Next we’ll try adding data to the map using different methods.
