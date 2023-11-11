---
name: Homework 8
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: Visualizations for Homework 8 
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Building Inventory Data Visualizations

## First Plot

Heatmap of Square Footage per Agency

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inventory.json" style="width: 100%"></vegachart>

For my first plot, I created a heatmap that shows the sqaure footage per different agencies. I set the max bins for this visualization to be 10. The differernt colors of the heatmap are based on the count of records of each agency. 


## Second Plot 

Scatter Plot of Year Constructed and Square Footage by Building Status 

<vegachart schema-url="{{ site.baseurl }}/assets/json/scatter_building.json" style="width: 100%"></vegachart>

In the second plot, I made a scatter plot that shows the relationship between the year a building was constructed and its square footage. The different colors also represent the building status of each point. I used the built in zoom capabilities so that users can take a closer look at each point on the plot. For interactivity, I added a dropdown so that users will be able to select which building status they want to find information on. Users can also hover over different scatter points and it will show the agency name, year constructed, and square footage.


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/sophiamatias/sophiamatias.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>

