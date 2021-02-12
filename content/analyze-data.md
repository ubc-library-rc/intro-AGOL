---
layout: default
title: Analyzing Data
nav_order: 5
has_children: true
---

## ANALYZING DATA

In ArcGIS Online, you can add data from the Living Atlas, curated by Esri, from web services produced by other agencies, or you can add your own data in [multiple data formats](https://storymaps.arcgis.com/stories/c9d52ddee8f040d0acb4d219598f7fb6).
 
In this section, we want to continue exploring COVID-19 data, and deaths due to COVID-19, in Canada. We saw that the John Hopkins data only has provincial-level data for Canada, so let's see if we can find data with more detail. 

It turns out there are some other data available about COVID-19 in Canada. Some provide data for download, and some sites proivde visualizations or maps with the data available. Below is a list of just some of the COVID-19 data resources.

[Esri COVID-19 Open Data](https://resources-covid19canada.hub.arcgis.com/pages/open-data)

[University of Toronto Libraries COVID-19 Data Resources](https://mdl.library.utoronto.ca/covid-19/resources)

[Flatten](https://www.flatten.ca/)

[COVID-19 in Canada](https://art-bd.shinyapps.io/covid19canada/)

[COVID-19 Canada Open Data Working Group](https://opencovid.ca/)

[Canada COVID-19 interactive growth rate explorer](https://mountainmath.ca/shiny/canada_covid-19/?_inputs_&level=%22province%22&metric=%22Confirmed%22&province=%2201%22&start_cutoff=100)

Because we're working in ArcGIS Online, let's take a look at a comprehensive [dataset](https://resources-covid19canada.hub.arcgis.com/datasets/health-region-summaries) that provides health region summaries from Esri's data hub for COVID-19 data in Canada.

The map at the top of this page shows the extent of the data, and the **Overview** tab below shows us all of the attributes associated with this dataset. Notice the population data by age available for this dataset. 

This will be useful for trying to visualize the relationship between death due to COVID-19 and age since we know that [vulnerability increases with age, particularly over 60 years](https://www.canada.ca/en/public-health/services/publications/diseases-conditions/vulnerable-populations-covid-19.html). [StatCan found that 52% of excess deaths in Canada from March to June 2020](https://www.ctvnews.ca/health/coronavirus/canadians-age-85-and-older-account-for-over-half-of-excess-deaths-amid-covid-19-statcan-1.5205790), assumed to be due to COVID-19, were among those 85 and older, which is a specific age category in this dataset.

Just under the map showing health region summaries at the top, there is a download button with a dropdown arrow. We see that this dataset is available in a number of different formats. To use this data in ArcGIS Online, we could download the data as a spreadsheet or a shapefile, but there are several reasons to use the data in ArcGIS Online without ever downloading it, which may require using a desktop GIS application to manipulate the data before adding it back to ArcGIS Online.

Good reasons to use data available online through Esri include:
- Popups that have already been configured appropriately
- Ability to create new fields and manipulate data using [Arcade](https://www.esri.com/arcgis-blog/products/apps/uncategorized/introducing-arcade/) expressions
- Curated data that would be difficult to find otherwise, like the the Health Region Summaries

Let's check and see whether we can add this dataset from ArcGIS Online itself to our map. 

*1*{: .circle .circle-blue} From the map, click the dropdown arrow next to the **Add** button and select **Search for Layers**.  

*2*{: .circle .circle-blue} Ensure you are searching ArcGIS Online by clicking the dropdown arrow and selecting **ArcGIS Online** below **Living Atlas** among the list of options. 

*3*{: .circle .circle-blue} Search for **health region summaries canada** and click the plus symbol to add **Health Region Summaries** to the map before clicking the back arrow at the top of the search box to see the content list for the map.

*4*{: .circle .circle-blue} If the layer automatically opens in symbology mode, click **OK** to accept the default for now.

*11*{: .circle .circle-blue} Now let's change the symbology. Click on the third icon from the left to open the **Change Style** window.

*12*{: .circle .circle-blue} From the dropdown arrow under **Choose an attribute to show**, scroll down to select **Deaths** again and then click **Add attribute** and select the custom field you created **2019 Total Pop 60 to 85 or Older**. THIS MAY NOT SHOW UP AND RELATIONSHIP OPTION DOESN'T SHOW UP WITH THIS. NEED TO TROUBLESHOOT.

Because we know that older people are at greater risk of dying with this coronavirus, we can expect there to be a relationship between these two variables.

We also see that once we select two attributes instead of one to display, different drawing styles become available. The default is the proportional symbology we previously used to show deaths from COVID-19 around the world.

*13*{: .circle .circle-blue} Scroll down until you see the **Relationship** option and click once this to see what happens to the symbology in the map.

What is referred to in ArcGIS Online as a Relationship symbology really refers to a [bivariate chloropleth map](https://www.joshuastevens.net/cartography/make-a-bivariate-choropleth-map/), which helps us understand the relationship between two variables. Since we know there is a relationship between deaths due to COVID-19 and age, this seems like an appropriate symbology to use. 

Now that we know we want to use a chloropleth map to illustrate this relationship, we first need to normalize the data, which we'll do in the next section.
