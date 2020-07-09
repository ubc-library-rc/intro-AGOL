---
layout: default
title: Symbology
nav_order: 4
parent: Create a Web Map
---

## SYMBOLOGY

To Do
{: .label .label-green }
Click on the third icon from the right underneath the **Deaths** layer called **Change Style**.

Click on **OPTIONS** under the **Location (Single Symbol)** window.

*1*{: .circle .circle-blue} In the next dialog, click on **Symbols**.
A dialog box will open.

From the dropdown arrow, select **Cartographic**.

Scroll down to select the symbol below. Accept the default size.

![cartoSymbol.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/cartoSymbol.jpg)

*2*{: .circle .circle-blue} Click **OK**.

Notice that you can also adjust the transparency of the layer and the visible range. 
For our purposes, we'll accept the defaults.

Click **OK**.

Then click **Done**.

The distribution of deaths across the world is now much more visible.

But because the data is represented differently depending on the country, the symbology does not accurately represent the number of deaths per country. As mentioned before, some countries have death counts by city, some by county, and some only at the country level.

Let's experiment with another kind of symbology.

*3*{: .circle .circle-blue} Click the ellipsis (the three dots) under the **Deaths** layer and select **Copy**.

This will create a copy of the **Deaths** layer. 

*4*{: .circle .circle-blue} Click the **Change Styles** icon again and click the **SELECT** button under **Heat Map**.

From the dropdown above, select **Deaths**. The default is **Location**.

Click **DONE**.

*5*{: .circle .circle-blue} Turn off the original **Deaths** layer by unchecking it.

The [**Heat Map**](https://www.gislounge.com/heat-maps-in-gis/) symbology represents higher densities by color and is a good way to be able to immediately visually locate the areas of greatest concentration of COVID-19-related deaths.

*6*{: .circle .circle-blue} Save your map.

In the next section you'll learn how to add your own data to a web map.
