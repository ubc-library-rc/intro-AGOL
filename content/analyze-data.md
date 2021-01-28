---
layout: default
title: Analyzing Data
nav_order: 5
has_children: true
---

## ANALYZING DATA

In ArcGIS Online, you can add data from the Living Atlas, curated by Esri, from web services produced by other agencies, or you can add your own data.

There are multiple data formats that can be added to an AGOL web map. 

 - [shapefile](https://desktop.arcgis.com/en/arcmap/latest/manage-data/shapefiles/what-is-a-shapefile.htm) - to be added to the map, the different components of the shapefile must be compressed into a ZIP archive
 - CSV or TXT files with optional address, place or coordinate locations (comma, semi-colon or tab delimited)
 - GPX (GPS Exchange Format)
 - [GeoJSON](https://geojson.org/) (open standard format for simple geographical features)
 
We want to zoom in on the map and explore the pandemic from a more localized perspective. Let's try and better understand COVID-19 data in Canada. 

In additon to the data curated by Johns Hopkins that we've been using so far, there are some other data available about COVID-19 in Canada. Some provide data for download, and some sites proivde visualizations or maps with the data available. Below is a list of just some of the COVID-19 data resources.

[Esri COVID-19 Open Data](https://resources-covid19canada.hub.arcgis.com/pages/open-data)

[University of Toronto Libraries COVID-19 Data Resources](https://mdl.library.utoronto.ca/covid-19/resources)

[Flatten](https://www.flatten.ca/)

[COVID-19 in Canada](https://art-bd.shinyapps.io/covid19canada/)

[COVID-19 Canada Open Data Working Group](https://opencovid.ca/)

[Canada COVID-19 interactive growth rate explorer](https://mountainmath.ca/shiny/canada_covid-19/?_inputs_&level=%22province%22&metric=%22Confirmed%22&province=%2201%22&start_cutoff=100)

Because we're working in ArcGIS Online, let's take a look at a comprehensive [dataset](https://resources-covid19canada.hub.arcgis.com/datasets/health-region-summaries) that provides health region summaries from Esri's data hub for COVID-19 data in Canada.

The map at the top of this page shows the extent of the data, and the **Overview** tab below shows us all of the attributes associated with this dataset. Notice the population data by age available for this dataset. This will be useful for trying to visualize the relationship between death due to COVID-19 and age since we know that [vulnerability increases with age, particularly over 60 years](https://www.canada.ca/en/public-health/services/publications/diseases-conditions/vulnerable-populations-covid-19.html).  

Below the attributes, Esri has also created web maps and web apps using certain data. We'll keep these in mind for the storymap we will be creating in a later section of this workshop.

Just under the map showing health region summaries at the top, there is a download button with a dropdown arrow. We see that this dataset is available in a number of different formats. To use this data in ArcGIS Online, we could download the data as a spreadsheet or a shapefile.

First let's check and see whether we can add this dataset from ArcGIS Online itself to our map, which would provide a dataset with a popup that has already been configured appropriately.

*1*{: .circle .circle-blue} From the map, click the dropdown arrow next to the **Add** button and select **Search for Layers**.  

*2*{: .circle .circle-blue} Ensure you are searching ArcGIS Online by clicking the dropdown arrow and selecting **ArcGIS Online** below **Living Atlas** among the list of options. 

*3*{: .circle .circle-blue} Search for **health region summaries canada** and click the plus symbol to add **Health Region Summaries** to the map before clicking the back arrow at the top of the search box to see the content list for the map.

*4*{: .circle .circle-blue} If the layer automatically opens in symbology mode, click **OK** to accept the default for now.

In order to continue exploring deaths due to COVID-19, we want to relate the number of deaths to the population 60 years and older. This attribute currently does not exist in the dataset, so first we need to add a custom expression to sum the values from attributes representing population in ages groups ranging from 60 to 65 to 85 and older.

*5*{: .circle .circle-blue} Click on the three dots below the **Health Region Summaries** layer in the **Contents** pane.

*6*{: .circle .circle-blue} Click on **Configure Pop-up** and then under **Attribute Expressions**, click on **Add**.

*7*{: .circle .circle-blue} Copy and paste the following expression to add another field which sums all of the values for populations ages 60 to 85 and older.

```json
    Sum($feature.Pop60to64_2019,$feature.Pop65to69_2019, $feature.Pop70to74_2019, $feature.Pop75to79_2019, $feature.Pop80to84_2019, $feature.Pop85Older)
```

*5*{: .circle .circle-blue} From the dropdown arrow, scroll down to select **Deaths** again and then click **Add attribute** and select **2019 Total Pop 85 or Older** because we know that with this coronavirus, older people are at greater risk of dying so we can expect there to be a relationship between these two variables.

Once you select two attributes to show, you'll see that different drawing styles become available. 

*6*{: .circle .circle-blue} Scroll down until you see the **Relationship** option and click once this to see what happens to the symbology in the map.

At first glance, the default classification scheme shows that there is a more significant relationship between these two variables in British Columbia, Alberta, Quebec and Ontario.

![quantile](https://raw.githubusercontent.com/ubc-library-rc/intro-AGOL/master/content/images/quantile.jpg)

*7*{: .circle .circle-blue} Select the **Relationship** option by clicking on it again and notice that the classification method is listed as Quantile.

ADD INFO ON CLASSIFICATION METHODS AND CHOOSE EQUAL INTERVAL?


You should have downloaded this data in preparation for our workshop, but in case you didn't, you can [download](https://opendata.vancouver.ca/explore/dataset/homeless-shelter-locations/download/?format=geojson&timezone=America/Los_Angeles&lang=en) it now. 

In the next section, we'll add this GeoJSON file of [homeless shelter locations](https://opendata.vancouver.ca/explore/dataset/homeless-shelter-locations/export/) to our AGOL map.

