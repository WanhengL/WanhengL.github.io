---
name: Example in Class
tools: [Python, HTML, vega-lite]
image: assets/pngs/unemployment.png
description: Ongoing example!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Example including vega-lite

Example that came with the template:
<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>

## Example from the vega-editor

Simple barplot specification:
<vegachart schema-url="{{ site.baseurl }}/assets/json/firstViz.json" style="width: 100%"></vegachart>

## Something more complicated with interactivity:
<vegachart schema-url="{{ site.baseurl }}/assets/json/unemployment.json" style="width: 100%"></vegachart>

## From a dictonary in Altair in Python
<vegachart schema-url="{{ site.baseurl }}/assets/json/chart1.json" style="width: 100%"></vegachart>

## Static side-by-side
<vegachart schema-url="{{ site.baseurl }}/assets/json/static_mobility.json" style="width: 100%"></vegachart>

## Interactive dashboard side-by-side
<vegachart schema-url="{{ site.baseurl }}/assets/json/interactive_mobility.json" style="width: 100%"></vegachart>

<!-- these are written in a combo of html and liquid --> 
<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

