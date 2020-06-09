---
layout: default
title: Title of page, will appear in left navigation menu
nav_order: 1
parent: create-a-web-map
---

To Do {: .label .label-green }
On the ribbon on the left, click the Add dropdown arrow and select Browse Living Atlas Layers. The [Living Atlas](https://livingatlas.arcgis.com/en/) is a large collection of geographic information compiled and created by [Esri.](https://www.esri.com/en-us/home) From the search bar, type “COVID-19 Canada” in the search bar to see what layers may be available. Click on “Coronavirus COVID-19 Cases V2.” An information dialogue will open with information about this layer.   

![add_LA_data}(https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/add_LA_data.png)

Scroll down to read about it. This layer is created and maintained by the Center for Systems Science and Engineering (CSSE) at the Johns Hopkins University, which is also maintaining the well known [Dashboard](https://coronavirus.jhu.edu/map.html) tracking COVID-19 cases and deaths across the world. This layer contains the same underlying data feeding that dashboard.

Click **Add to Map**, then click the back arrow above the Add Data search bar to return to the Contents pane.

If your extent is still showing the University of British Columbia campus, zoom out using the scroll on your mouse or by clicking the  minus button in the upper left until you see the single red circle representing British Columbia. If you'd like, you can zoom out to show the extent of the data for the entire world.

Click on **Content** in the upper left to see the different layers currently in the map. 
![content](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content.jpg)

The **Topographic** layer represents the default basemap whenever you open a web map in AGOL. Let's change the basemap to something that looks better with the COVID-19 data.

To Do {: .label .label-green }
From the upper left, click on **Basemap** and select the **Light Gray Canvas**.
Click on the **Save** dropdown arrow in the ribbon above the map and select **Save**.

Now let's explore different ways of discovering the underlying data.

To Do {: .label .label-green }
Click on the red circle located in British Columbia to view a pop-up containing information about the number of confirmed, recovered, deaths, and active cases of COVID-19.
![covidCases.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/covidCases.jpg)

You'll notice that there are three entries for British Columbia with the same information. In the **Contents** pane on the left, there are four layers associated with the data we added from the Living Atlas. Uncheck the blue checkmarks next to every layer except the layer representing **Deaths**. 
You'll see that this layer is depicted using the symbol of a black X.

To Do {: .label .label-green }


You may also notice that the data for Canada is less detailed than the data for the United States. Whereas in Canada, data is only reported at the province level in this dataset, in the U.S. it is reported at the state and county level. 
