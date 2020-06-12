---
layout: default
title: Explore Data Layers
nav_order: 3
parent: Create a Web Map
---

To Do
{: .label .label-green }
Click on the red circle located in British Columbia to view a pop-up containing information about the number of confirmed, recovered, deaths, and active cases of COVID-19.

![covidCases.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/covidCases.jpg)

You'll notice that there are three entries for British Columbia with the same information. 

In the **Contents** pane on the left, there are four layers associated with the data we added from the Living Atlas. 

Uncheck the blue checkmarks next to every layer except the layer representing **Deaths**. You'll see that this layer is depicted using the symbol of a black X.

To Do
{: .label .label-green }
Click on the first layer in the **Contents** pane to explore the data and the tools associated with each layer.

![deathsLyr.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/deathsLyr.jpg)

The far left icon associated with the **Deaths** layer represents the legend. If you click on it, the legend symbols will appear below the layer.

Hovering over the next icon reveals that clicking on this will open the attribute table. The table, which contains the underlying data in spreadsheet form, will open at the bottom of your screen. You can click on the grey line at the top center to drag the table up in order to see more rows at one time.

To Do
{: .label .label-green }
Click on the first row in the table and then click the three grey lines in the upper left of the table and select **Center on Selection**.
Then click **Clear Selection**.

Next, from the same place, select **Filter**. This will open a window where you can customize an expression to select only the records you specify.
Let's filter the data in order to find those places in the world that have surpassed 10,000 deaths from COVID-19.
From the dropdown arrow on the left, select the **Deaths** field.
From the dropdown arrow in the centre, select **is greater than**.
In the far right field, type in **10000**.
Then click **APPLY FILTER AND ZOOM TO**.
Close the attribute table.

Around the world, Sao Paulo, Brazil, the UK, New York, and Lombardia, Italy have all surpassed 10,000 deaths from COVID-19.

You may notice that the black X symobilizing the **Deaths** layer is very hard to see. In the next section, we will change the symbology of this layer to make it more visible.



