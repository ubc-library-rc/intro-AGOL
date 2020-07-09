---
layout: default
title: Configure Your Own Data
nav_order: 1
parent: Add Your Own Data
---

## CONFIGURE YOUR OWN DATA

To Do
{: .label .label-green }
From your web map, click the **Add** dropdown arrow and select **Add Layer From File**.

*1*{: .circle .circle-blue} Upload the GeoJSON file and click **IMPORT LAYER**.

You will automtically be prompted to change the symbology. 
We want to know which homeless shelters are able to accomodate pets.

*2*{: .circle .circle-blue} Click the dropdown arrow and select **Pets**. 

*3*{: .circle .circle-blue} Click on **Options** under **Types (Unique symbols)**.
There are default colors representing yes/no values as well as a count of each.
Let's change the symbology.

*4*{: .circle .circle-blue} Click on the red dot currently representing those shelters where pets are not accepted.

*5*{: .circle .circle-blue} Select **SHAPE** and then from the dropdown arrow, select **General Infrastructure**. 

*6*{: .circle .circle-blue} Navigate to the house symbol seen below and increase the size to 20.

![blueHouse.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/blueHouse.jpg)

*7*{: .circle .circle-blue} Next click on the blue dot representing shelters where pets *are* accepted.

*8*{: .circle .circle-blue} Select **SHAPE** and **Public Safety** from the dropdown and select the grey dog as seen below. 

*9*{: .circle .circle-blue} Increase the size to 20.

![greydog.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/greyDog.jpg)

*10*{: .circle .circle-blue} Click **OK** and then **DONE**.

*11*{: .circle .circle-blue} Save the map.

Next change the name of the layer in the **Content** pane.

*12*{: .circle .circle-blue} Click the ellipsis underneath the **homeless-shelter-locations** layer.

*13*{: .circle .circle-blue} Select **Rename** and type in **Homeless Shelters That Allow Pets**.

*14*{: .circle .circle-blue} Click on one of the symbols in the map representing locations that allow pets to see the popup.

![popup.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/popup.jpg)

Let's edit the popup to reconfigure the way the information appears when somebody clicks on a symbol.

*15*{: .circle .circle-blue} Click on the ellipsis underneath the layer in the **Content** pane. 

*16*{: .circle .circle-blue} Select **Configure Pop-up**.

*17*{: .circle .circle-blue} In the **Configure Pop-up**, first add a title: **Homeless Shelter**.

*18*{: .circle .circle-blue} Click on **Configure Attributes.**

The **Configure Attributes** dialog window will open. 

*19*{: .circle .circle-blue} Click on **category** in the **Field Alias** and change it to **Category.**

This field describes whether the shelter accepts all adults, only youth, or only men.

Remember that you can open the attribute table to explore the values in the different fields.

*20*{: .circle .circle-blue} Change the following fields under **Field Alias.**


| Original  | Change to |
| ------------- | ------------- |
| facility  | Facility Name |
| carts  | Cart |
| phone  | Phone Number |
| pets  | Pets Allowed |
| meals  | Meals Offered |
| geo_local_area  | Neighborhood |

*21*{: .circle .circle-blue} Click **OK** and then **OK** again. 
Don't forget to save your map to save the changes you just made.

Now when you click on one of the symbols in the map, the popup will look like this.

![popup_after.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/popup_after.jpg)

As you can see, creating a web map using ArcGIS Online provides a number of preconfigured settings and tools while still giving the user the option to add data, change basemaps, customize symbology, filter the data, and configure popups, among other things.

Using ArcGIS Online, you can also create [StoryMaps](https://storymaps.arcgis.com/stories) and more powerful, customized interactive maps using [WebApp Builder](https://www.esri.com/en-us/arcgis/products/web-appbuilder/overview).

In the next and final section of this workshop, we'll incorporate the web map we just created into a StoryMap.









