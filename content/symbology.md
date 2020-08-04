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

From the default **Shapes**, select the first symbol, a black dot.

Change the size to **12 points**.

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

*4*{: .circle .circle-blue} Click the **Change Styles** icon again and select **Deaths** from the dropdown under **Choose an attribute to show**.

This will prompt the appearance of different symbology options. 

By default **Counts and Amounts (Size)** is selected.

These are also called [proportional symbols](https://pro.arcgis.com/en/pro-app/help/mapping/layer-properties/proportional-symbology.htm).
- Maps using these are a kind of thematic map used to show relative differences in quantities

You can make adjustments to this symbology, but we'll accept the defaults for now.

Click **DONE**.

*5*{: .circle .circle-blue} Turn off the original **Deaths** layer by unchecking it.

The [proportional](http://wiki.gis.com/wiki/index.php/Proportional_symbol_map) symbology is a good way to be able to immediately visually locate the areas with the greatest numbers of COVID-19-related deaths.

Be aware that it is easy to misrepresent data based on the symbology you choose to use. It is worth doing some research to help you decide what symbology choice makes the most sense.

[ArcGIS Online Change Style Quick Reference](https://doc.arcgis.com/en/arcgis-online/create-maps/change-style.htm)

*6*{: .circle .circle-blue} Save your map.

![propMap](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/propMap.jpg)

Your map should end up looking something like [this web map](https://arcg.is/8i8uv0).

In the next section you'll learn how to add your own data to a web map.
