---
name: Illinois Building Inventory
tools: [Python, HTML, vega-lite]
image: assets/pngs/ibuildings.png
description: This projects shows some interactive visualization for the Illinois Buildings Inventory dataset.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Illinois Building Inventory

This graph shows the relationship between the [Year Constructed] and [Square Footage] for five selected cities near U of I.

<vegachart schema-url="{{ site.baseurl }}/assets/json/ibuildings.json" style="width: 100%"></vegachart>




<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

