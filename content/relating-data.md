---
layout: default
title: Relating Data
nav_order: 2
parent: Analyzing Data
---

## RELATING DATA

One of the strengths of the **Health Region Summaries** data is the age-related information that comes with it. While it does not tell us COVID-19 deaths by age, we can create a map that shows the relationship between two variables, deaths and the population 85 years and older.

You may remember that we created a copy of this dataset in our web map. If you haven't done so already, we'll start off by renaming it. 

To Do
{: .label .label-green }
Uncheck all layers except the copy of the **Health Region Summaries** data you made and rename it to **Deaths Per Pop & Pop 85 +**. Save your map.

Let's play around with the symbology to see how we can best show the relationship between deaths and the most vulnerable age group to COVID-19, those 85 years and older.

*1*{: .circle .circle-blue}  Open the symbology by clickng on the third icon from the left to open the **Change Style** window.

*2*{: .circle .circle-blue} From the dropdown arrow under **Choose an attribute to show**, scroll down to select **Deaths** and then click **Add attribute** and select the custom field you created **2019 Total Pop 85 or Older**.

We also see that once we select two attributes instead of one to display, different drawing styles become available. The default is the proportional symbology we previously used to show deaths from COVID-19 around the world.

*13*{: .circle .circle-blue} Scroll down until you see the **Relationship** option and click once this to see what happens to the symbology in the map.

What is referred to in ArcGIS Online as a Relationship symbology really refers to a [bivariate chloropleth map](https://www.joshuastevens.net/cartography/make-a-bivariate-choropleth-map/), which helps us understand the relationship between two variables. Since we know there is a relationship between deaths due to COVID-19 and age, this seems like an appropriate symbology to use. 

*1*{: .circle .circle-blue} 

We plan on creating a chloropleth symbology to illustrate the relationship between two variables, deaths and the population 60 to 85 years and older. Data normalization refers to using rates or percentages instead of absolute values, which is important because each health region in our map is a different size with different number of people living in each region. Normalization allows us to better compare rates of death across areas normalizing for population. 

This data layer uses [chloropleth](http://wiki.gis.com/wiki/index.php/Choropleth_map) symbology, in which areas are shaded or patterned proportionally to the value of a variable measured for each area.

- The variable is usually quantitative
- A color is associated with an attribute value
- It's a method for showing how a measurement varies across a geographic area

You can read more about and see examples of chloropleth [maps](https://arcg.is/15Xffe).

At first glance, the default classification scheme shows that there is a more significant relationship between these two variables in British Columbia, Alberta, Quebec and Ontario.

![quantile](https://raw.githubusercontent.com/ubc-library-rc/intro-AGOL/master/content/images/quantile.jpg)

*7*{: .circle .circle-blue} Select the **Relationship** option by clicking on it again and notice that the classification method is listed as Quantile.

ADD INFO ON CLASSIFICATION METHODS 

In the next section, we'll create a [story map](https://storymaps.arcgis.com/stories) in order to tell a visually rich story of COVID-19 deaths in Canada.

### ADDITIONAL RESOURCES

[Mapping coronavirus, responsibly](https://www.esri.com/arcgis-blog/products/product/mapping/mapping-coronavirus-responsibly/)

[ArcGIS Online Relationship Style](https://enterprise.arcgis.com/en/portal/latest/use/style-numbers.htm#ESRI_SECTION1_C7FAB061D60344CAB6AC9A190DAED1D2)

[Telling the Truth - Data classification](http://uxblog.idvsolutions.com/2011/10/telling-truth.html)

[Better Breaks Define Your Map’s Purpose](https://www.esri.com/arcgis-blog/products/arcgis-online/mapping/better-breaks-define-your-maps-purpose/)

[Evaluation of Methods for Classifying Epidemiological Data on Chloropleth Maps in Series](http://php.scripts.psu.edu/users/c/a/cab38/Pub_scans/Brewer-Pickle_2002_Epi-Choropleth-Classing_Annals.pdf)















