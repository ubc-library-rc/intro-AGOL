---
layout: default
title: Analyzing Data
nav_order: 6
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

This will be useful for trying to visualize the relationship between death due to COVID-19 and age since we know that [vulnerability increases with age, particularly over 60 years](https://www.canada.ca/en/public-health/services/publications/diseases-conditions/vulnerable-populations-covid-19.html).

[StatCan found that 52% of excess deaths in Canada from March to June 2020](https://www.ctvnews.ca/health/coronavirus/canadians-age-85-and-older-account-for-over-half-of-excess-deaths-amid-covid-19-statcan-1.5205790), assumed to be due to COVID-19, were among those 85 and older, which is a specific age category in this dataset.

Just under the map showing health region summaries at the top, there is a download button with a dropdown arrow. We see that this dataset is available in a number of different formats. To use this data in ArcGIS Online, we could download the data as a spreadsheet or a shapefile, but there are several reasons to use the data in ArcGIS Online without ever downloading it, which may require using a desktop GIS application to manipulate the data before adding it back to ArcGIS Online.

Good reasons to use data available online through Esri include:
- Popups that have already been configured appropriately.
- Ability to create new fields and manipulate data using [Arcade](https://www.esri.com/arcgis-blog/products/apps/uncategorized/introducing-arcade/) expressions.
- Curated data that would be difficult to find otherwise, like the Health Region Summaries.

We'll add this dataset as a [web service](https://doc.arcgis.com/en/arcgis-online/reference/arcgis-server-services.htm) hosted by Esri in ArcGIS Online to our map.

*1*{: .circle .circle-blue} From the map, click the dropdown arrow next to the **Add** button and select **Add layer from web**.  

*2*{: .circle .circle-blue} Copy and paste the following URL in the box and click **OK**.

```json
    (https://services9.arcgis.com/pJENMVYPQqZZe20v/arcgis/rest/services/NewHybridRegionalHeathBoundaries/FeatureServer)
```

This layer may have a visibility range associated with it that requires you to zoom in to see it.

*3*{: .circle .circle-blue} Click on the ellipsis on the right for this new layer and select **Set Visibility Range** and drag the slider on the left all the way to the left. Save your map.

*4*{: .circle .circle-blue} If the layer automatically opens in symbology mode, click **OK** to accept the default for now.

Let's try and understand the severity of COVID-19 in Canada using this data.

[Two measures used to assess severity of an infectious disease](https://www.who.int/news-room/commentaries/detail/estimating-mortality-from-covid-19) are the infection fatality ratio (IFR) and the case fatality ratio (CFR). We only have data to calculate the CFR.

*5*{: .circle .circle-blue} First create a copy of this layer like we did in a previous step so we can create different layers with the data (hint: ellipsis > Copy).

*6*{: .circle .circle-blue} Using the original Health Region Summaries layer, click on the icon third from the left representing symbology, or **Change Style.**

We will use a calculation for CFR [restricting our analysis to resolved cases](https://www.who.int/news-room/commentaries/detail/estimating-mortality-from-covid-19) which is represented by the formula below because this is meant to better represent an ongoing epidemic. After the pandemic is over, it will be more appropriate to use a formula which takes the number of deaths divided by the number of cases and multiplies it by 100.

![CFR.jpg](../images/CFR_1.jpg)

*7*{: .circle .circle-blue} In the **Change Style** window, click the dropdown arrow under **Choose an attribute to show**.

*8*{: .circle .circle-blue} Select **Custom expression** at the very bottom. This will open a window where you can use the Arcade language to build expressions.

*9*{: .circle .circle-blue} Copy and paste the following expression in the window.

```json
    ($feature.Deaths / ($feature.Deaths + $feature.Recovered) * 100)
```

*10*{: .circle .circle-blue} Click the **Edit** icon near the word **Custom** and rename this new field to **Case Fatality Ratio**. Click **OK**.

The symbology defaults to proportional symbols, but these overwhelm certain areas of the map. One option might be to resize these symbols, but we are going to experiment with [choropleth](http://wiki.gis.com/wiki/index.php/Choropleth_map) symbology, in which areas are shaded or patterned proportionally to the value of a variable measured for each area, to show the Case Fatality Ratio.

In choropleth mapping:
- The variable is usually quantitative.
- A color is associated with an attribute value.
- the shading illustrates how a measurement varies across a geographic area.

You can read more about and see examples of choropleth [maps](https://arcg.is/15Xffe).

*11*{: .circle .circle-blue} Click on **Counts and Amounts**, and you'll notice a dark cluster of health regions in eastern Canada.

The default symbology uses **High to Low** and provides a range where 3.3% CFR and higher is given the full dark purple color and those with a CFR of .5% or lower is given the full yellow color. Hovering over the *x* shows the average CFR in each health region, 1.9%.

*12*{: .circle .circle-blue} Select the **Above and Below** theme from the dropdown menu and notice how the algorithm selects breaks in the data that are more in line with what the histogram is telling us about the how the data is grouped.

This setting is telling us that green health regions on the map have lower than normal CFR rates and the darker red health regions have higher than normal CFR rates.

I think the Above and Below option is a better representation of this data. What do you think?

To learn more about these different themes and also about whether to classify data or not, check out this Esri blog post [Better Breaks Define Your Map’s Purpose](https://www.esri.com/arcgis-blog/products/arcgis-online/mapping/better-breaks-define-your-maps-purpose/).

Let's experiment with classifying the data.

*13*{: .circle .circle-blue} Check the **Classify Data** box, which defaults to using a [Natural Breaks](http://wiki.gis.com/wiki/index.php/Jenks_Natural_Breaks_Classification) classification method which attemps to mathematically find "natural" classes that group together in a dataset. It also defaults to four classes.

You'll notice that the range for the fourth class is largest, from 3.9% to 8%.

*14*{: .circle .circle-blue} Now select the [Quantile](http://wiki.gis.com/wiki/index.php/Quantile) classification method, which creates classes with the same number of features.

In this case, the fourth class represents a range from under 2.77%-8%. Because classifying the data does not provide any additional meaningful detail and because we're not asking specific questions related to certain thresholds, it makes more sense to leave the data unclassified. What we can say is that the case fatality ratio is much higher in certain health regions in eastern Canada than throughout the rest of Canada.

*15*{: .circle .circle-blue} Uncheck the **Classify** button and ensure that **Above and Below** is selected, click **OK** and then **Done**.

Let's configure the popups to include the CFR.

*16*{: .circle .circle-blue} Select **Configure Popup** by clicking on the ellipsis and click on **ADD** under **Attribute Expressions**.

*17*{: .circle .circle-blue} Edit the name to be **Case Fatality Ratio (%)**.

*18*{: .circle .circle-blue} Copy and paste the following expression in the expression window and then click **OK**

```json
    ($feature.Deaths / ($feature.Deaths + $feature.Recovered) * 100)
```
Now when you click on the popup, the CFR will appear at the bottom.

Your map should look something like the image below, but keep in mind the data is constantly changing, so it won't look exactly the same.

![aboveBelow.png](../images/aboveBelow.png)

It's important to keep in mind that the majority of Canada's population lives clustered along the southern belt of Canada, closer to the U.S. border. So a map like this does not do a good job of representing smaller populations in more northern regions of the country. These health regions summaries are better at representing what's happening in more populated areas.

In the next section, we'll add some population data to help contextualize the CFR in these locations.
