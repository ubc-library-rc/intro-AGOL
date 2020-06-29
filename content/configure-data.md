---
layout: default
title: Configure Your Own Data
nav_order: 1
parent: Add Your Own Data
---

## CONFIGURE YOUR OWN DATA

To Do
{: .label .label-green }
**Step 1:** From your web map, click the **Add** dropdown arrow and select **Add Layer From File**.

**Step 1a:** Upload the geoJSON file and click **IMPORT LAYER**.

You will automtically be prompted to change the symbology. 
We are concerned wth which homeless shelters are able to accomodate pets.

**Step 2:** Click the dropdown arrow and select **Pets**. 

**Step 3:** Click on **Options** under **Types (Unique symbols)**.
There are default colors representing yes/no values as well as a count of each.
Let's change the symbology.

**Step 4:** Click on the red dot currently representing those shelters where pets are not accepted.

**Step 5:** Select **SHAPE** and then from the dropdown arrow, select **General Infrastructure**. 

**Step 5a:** Navigate to the house symbol seen below and increase the size to 20.

![blueHouse.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/blueHouse.jpg)

**Step 6:** Next click on the blue dot representing shelters where pets *are* accepted.

**6a:** Select **SHAPE** and **Public Safety** from the dropdown and select the grey dog as seen below. 

**6b:** Increase the size to 20.

![greydog.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/greyDog.jpg)

**Step 7:** Click **OK** and then **DONE**.

**Step 8:** Save the map.

Next change the name of the layer in the **Content** pane.

**Step 9:**  Click the ellipsis underneath the **homeless-shelter-locations** layer.

**Step 9a:** Select **Rename** and type in **Homeless Shelters That Allow Pets**.

**Step 10:** Click on one of the symbols in the map representing locations that allow pets to see the popup.

![popup.jpg](https://raw.githubusercontent.com/fiddleHeads/intro-AGOL/master/content/images/popup.jpg)

Let's edit the popup to reconfigure the way the information appears when somebody clicks on a symbol.

**Step 11:** Click on the ellipsis underneath the layer in the **Content** pane. 

**Step 12:** Select **Configure Pop-up**.

**Step 13:** In the **Configure Pop-up**, first add a title: **Homeless Shelter**.

**Step 13a:** Click on **Configure Attributes.**

The **Configure Attributes** dialog window will open. 

**Step 13b:** Click on **category** in the **Field Alias** and change it to **Category.**

This field describes whether the shelter accepts all adults, only youth, or only men.

Remember that you can open the attribute table to explore the values in the different fields.

**Step 13c:** Click on **facility** and change it to **Facility Name.**

**Step 13d:** Change the following categories under **Field Alias.**


| Original  | Change to |
| ------------- | ------------- |
| carts  | Cart |
| phone  | Phone Number |
| pets  | Pets Allowed |
| meals  | Meals Offered |
| geo_local_area  | Neighborhood |








