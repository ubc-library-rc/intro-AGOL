---
layout: default
title: Add Population Data
nav_order: 1
parent: Analyzing Data
---

## ADD POPULATION DATA

Just as we did in the first exercise, we can search for layers in ArcGIS Online that make our map more meaningful.

Census data from [Statistics Canada](https://open.canada.ca/data/en/dataset/3cf36302-1060-444e-988a-d97b6db5ad240) is normally a great place to find population information, but it's also usually distributed by area, whether Census subdivisions or dissemination areas. Two layers of polygons stacked on top of one another are difficult to view.

[Agriculture and Agri-Food Canada](https://www.agr.gc.ca/eng/agriculture-and-agri-food-canada/?id=1395690825741) has a robust [ArcGIS Online presence](http://bit.ly/16o91lM), and they also happen to publish population data in a way more useful for our purposes. They host an ArcGIS Online layer of the [Canadian Ecumene Database](https://open.canada.ca/data/en/dataset/3f599fcb-8d77-4dbb-8b1e-d3f27f932a4b), a database produced by Natural Resources Canada and representing populated places. Ecumene is a word meaning "inhabited lands."

Let's see if we can find and add this dataset to our web map.

To Do
{: .label .label-green }
From your web map, click the **Add** dropdown arrow and select **Search for Layers**. From the dropdown arrow, make sure **ArcGIS Online** is selected.

*1*{: .circle .circle-blue} In the search box, type **canada population ecumene** and click the plus sign next to two layers for comparison. **The Canadian Ecumene (CanEcumene) 2.0 GIS Database** and **Populated Places - Canadian Ecumene**. Click the back arrow to see the contents in your map again.

The latter layer is produced by Esri Canada using data from The Canadian Ecumene GIS Database. Uncheck this layer in the Table of Contents for now.

You'll notice that the The Canadian Ecumene (CanEcumene) 2.0 GIS Database is automatically located toward the bottom of your contents list and cannot be moved up or down. This means that we will be unable to view the data unless we change the transparency of our Case Fatality Ratio (CFR) layer.

*2*{: .circle .circle-blue} Click on the CFR layer and then on the ellipsis and select **Transparency** from the dropdown. Play around with the slider to view different transparencies and position it around 25%.

*3*{: .circle .circle-blue} Click on the **The Canadian Ecumene (CanEcumene) 2.0 GIS Database** layer to expand it and uncheck all but **Populated Places.*

Even with the transparency, this makes for a messy map.

*4*{: .circle .circle-blue} Uncheck **Populated Places** and check **Populated Places Area** instead.

This is less messy, still provides a sense of densely populated areas, but is hard to see.

*5*{: .circle .circle-blue} Uncheck the whole layer and check the box next to the other layer we added from ArcGIS Online, the **Populated Places - Canadian Ecumene** layer.

This is the same data as the **Populated Places Area** from the Database layer, but the difference is we're able to move this layer above our CFR layer for better visbility.

*6*{: .circle .circle-blue} If it's not already at the top in your Table of Contents, hover over the left side of the layer with your cursor and then click on the three vertical dots to move it to the top. Make sure it is checked on.

*7*{: .circle .circle-blue} You can remove the **The Canadian Ecumene (CanEcumene) 2.0 GIS Database** layer from the map and save your map.

*8*{: .circle .circle-blue} We no longer need our CFR layer to have any transparency, so you can change that back to 0%.

You'll notice that the default symobology for the **Populated Places** layer is red, which is a colour I recommend using sparingly and with intention in maps. In this case, it's also hard to see.

*9*{: .circle .circle-blue} Open the symbology (Change Style) for this layer and click on **OPTIONS** under **Select a drawing style** and then on the word **Symbols**.

*10*{: .circle .circle-blue} In the editable box that has a number with a # symbol in front of it, copy and paste #008387 and click **OK**, then **OK** again, then **DONE**, then save your map.

This green colour is more neutral and also provides decent contrast with the symbology from our CFR layer. 

This population data provides a helpful visualization of how population is distributed across Canada, and we can see that generally speaking, areas with greater population densities have a higher case fatality ratio.

In the next section, we'll compare two variables using what's called a [bivariate chloropleth map](https://www.joshuastevens.net/cartography/make-a-bivariate-choropleth-map/).




