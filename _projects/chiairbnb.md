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

## Select an area and see the price ranges

<vegachart schema-url="{{ site.baseurl }}/assets/json/chiairbnb.json" style="width: 100%"></vegachart>

## Related Contextual Visualization

### Chicago Crime Map

<img src="{{ site.baseurl }}/assets/pngs/chicrime.png" alt="Chicago Crime Map">

CLEARMap. (n.d.). https://gis.chicagopolice.org/ 

### Chicago Attraction Map For Tourists

<img src="{{ site.baseurl }}/assets/pngs/chicagotour.png" alt="Chicago Attractions Map">

chicagomap360.com. (n.d.). Map of chicago tourist: Attractions and monuments of Chicago. https://chicagomap360.com/chicago-tourist-map 

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

