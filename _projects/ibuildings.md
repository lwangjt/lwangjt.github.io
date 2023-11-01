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

Building Status Distribution for Illinoic County

<vegachart schema-url="{{ site.baseurl }}/assets/json/altair_ctbuilding.json" style="width: 100%"></vegachart>

* This graph is describing different types of building status per Illinois county. The building status includes "in-progress, in-use, abandoned" and are arregacated based on count. 
* Because the data is mainly focusing on the categorical variables, a bar plot is applied to aggregate different building status for every Illinoid county. The "paired" colormap is used while different choices are tried and "paris" is the most optimal one since the "in-progress" count is relatively low for all counties and "paris" darken the "in-progress" bars. 
* No imputing or dropping is applied to the original datasets since the aggreagating does not require a clean datasets. Aggreagating is done by applying through the encoding of y within Altair.
* This graph connects to the previous plots as I included more counties instead of the surrounding cities near U of I which makes the plot to contain more information.


Year Constructed vs Square Footage for Cities near U of I

<vegachart schema-url="{{ site.baseurl }}/assets/json/altair_ctsqft.json" style="width: 100%"></vegachart>

* This graph is describing the relationship between "Square_Footage" and "Year" for  cities around UIUC. Each colored line represent an individual city.
* Because the data is mainly focusing on the quantitative variables, a line plot is applied to transitions of buildings' square footage and its year of construction. This design could display a smoother transition between time periods as well as constract between cities.
* Filtering is applied to the original dataset. Firstly, I subset the dataset to contain only 5 cities around UIUC. Secondly, I threw out the rows that contain 0 as their "Year_Constructed".
* This graph connects to the previous plots as I limited the number of cities to only the cities near UIUC and seperate them into different line. 


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/lwangjt/lwangjt.github.io/blob/main/assets/json/altair_ctbuilding.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/lwangjt/lwangjt.github.io/blob/main/python_notebooks/ibuilding.ipynb" text="The Analysis" %}
</div>

