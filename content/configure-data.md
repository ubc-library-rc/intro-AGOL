---
layout: default
title: Add and Configure Your Own Data
nav_order: 1
parent: Add Your Own Data
---

## ADD AND CONFIGURE YOUR OWN DATA

To Do
{: .label .label-green }
From your web map, click the **Add** dropdown arrow and select **Add Layer From File**.

Upload the geoJSON file and click **IMPORT LAYER**.

You will automtically be prompted to change the symbology. 
We are concerned wth which homeless shelters are able to accomodate pets.

Click the dropdown arrow and select **Pets**. 

Click on **Options** under **Types (Unique symbols)**.
There are default colors representing yes/no values as well as a count of each.
Let's change the symbology.

Click on the red dot currently representing those shelters where pets are not accepted.
Select **SHAPE** and then from the dropdown arrow, select **General Infrastructure**. 
Navigate to the house symbol seen below and increase the size to 20.

![blueHouse.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/blueHouse.jpg)

Next click on the blue dot representing shelters where pets *are* accepted.
Select **SHAPE** and **Public Safety** from the dropdown and select the grey dog as seen below. 
Increase the size to 20.

![greydog.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/greyDog.jpg)

Click **OK** and then **DONE**.
Save the map.

Next change the name of the layer in the **Content** pane.
Click the ellipsis underneath the **homeless-shelter-locations** layer.
Select **Rename** and type in **Homeless Shelters That Allow Pets**.

Click on one of the symbols in the map representing locations that allow pets to see the popup.

![popup.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/popup.jpg)

Let's edit the popup to reconfigure the way the information appears when somebody clicks on a symbol.

Click on the ellipsis underneath the layer in the **Content** pane. 
Select **Configure Pop-up**.

In the **Configure Pop-up**, first add a title: **Homeless Shelter**.




