---
name: Rilakuma Color Distribution
tools: [Python, HTML, vega-lite]
image: assets/pngs/rila.jpg
description: This projects shows the color distribution of similar Rilakuma pictures.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
--- 


# Rilakuma Color Distribution

<img src="{{ site.baseurl }}/assets/pngs/color1.png" alt="color1">

<img src="{{ site.baseurl }}/assets/pngs/color2.png" alt="color2">

<img src="{{ site.baseurl }}/assets/pngs/color3.png" alt="color3">

<img src="{{ site.baseurl }}/assets/pngs/colorall.png" alt="colorall">
<!-- these are written in a combo of html and liquid --> 


<div class="left">
{% include elements/button.html link="https://github.com/lwangjt/datasets/tree/main/rilakuma" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/lwangjt/lwangjt.github.io/blob/main/python_notebooks/rilakuma.ipynb" text="The Analysis" %}
</div>

