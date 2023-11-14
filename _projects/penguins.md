---
name: Palmer's Penguins
tools: [Python, HTML, vega-lite]
image: assets/pngs/penguins.png
description: Some visualization and clustering for Palmer's penguins
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


## Flipper length vs Body mass

<vegachart schema-url="{{ site.baseurl }}/assets/json/combined_penguin.json" style="width: 100%"></vegachart>

## Body mass vs Species

<vegachart schema-url="{{ site.baseurl }}/assets/json/bodyspecies.json" style="width: 100%"></vegachart>

## Flipper length vs Body mass

<vegachart schema-url="{{ site.baseurl }}/assets/json/flipbody.json" style="width: 100%"></vegachart>

## Bill length vs Flipper length

<vegachart schema-url="{{ site.baseurl }}/assets/json/billflipper.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

