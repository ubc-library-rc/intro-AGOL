---
layout: default
title: Data Normalization and Classification
nav_order: 2
parent: Analyzing Data
---

## DATA NORMALIZATION AND CLASSIFICATION

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















