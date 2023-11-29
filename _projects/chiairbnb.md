---
name: Chicago Airbnb Listings
tools: [Python, HTML, vega-lite]
image: assets/pngs/chicagoairbnb.png
description: Find Your Affordable Airbnb in Chicago
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

Done by Lisa Wang

## Chicago Airbnb Listings & Price Ranges
### Select an area and see the price ranges

<vegachart schema-url="{{ site.baseurl }}/assets/json/chicagoairbnb.json" style="width: 100%"></vegachart>

### Analysis
* In this visualization, a scatter plot is shown on the chicago basemap, representing all the Chicago airbnb listing places using their longtitude and latitude information. When the user make a selection interval on the scatter plot on the top, a corresponding histogram showing the frequency of different price range will show up. The histogram encodes the count of the corresponding price range in the selected scatted (airbnb listing). 
* The contextual dataset here is the boundary.geojson which has the geographic boundary map of the Chicago city  (found at. https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Neighborhoods/bbvz-uum9). This is useful in this case because the user could select the area where they like according to the neighborhood or the approximate location of the map. I also included this as a base layer in the Chicago boundary driven plot because this could provide the audience with a better idea about where they are selecting from.
* The listing.csv mainly contains two information that I used. The first is the individual row there, representing each Chicago airbnb listing. The second information or feature that I used is the price_range feature which I created based on the price column which can be considered as a categorical variable because I manually seperated all the prices into three bins (<100, 100-300, >300).
* The boundary.geojson is a geographical data which contains the information of the boundary of chicago neighborhoods. Each row represents a different chicago neighborhood with corresponding geographic informaiton (longtitude, latitude), which make it useful where I added is as a basemap to the scatterplot that I created.


## Related Contextual Visualization

<div class="row">
  <div class="column">
    <img src="{{ site.baseurl }}/assets/pngs/chicrime.png" alt="Chicago Crime Map">
  </div>
  <div class="column">
    <img src="{{ site.baseurl }}/assets/pngs/chicagotour.png" alt="Chicago Attractions Map">
  </div>
</div>

<p>Left: <strong>{{ Chicago Crime Map}}</strong></p>

<p>Right: <strong>{{ Chicago Attractions Map}}</strong></p>

**Source(left to right):**

CLEARMap. (n.d.). https://gis.chicagopolice.org/ 

chicagomap360.com. (n.d.). Map of chicago tourist: Attractions and monuments of Chicago. https://chicagomap360.com/chicago-tourist-map


<div class="left">
{% include elements/button.html link="https://github.com/lwangjt/datasets/blob/main/chicago_airbnb/listings.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/lwangjt/lwangjt.github.io/blob/main/python_notebooks/chiairbnb.ipynb" text="The Analysis" %}
</div>

