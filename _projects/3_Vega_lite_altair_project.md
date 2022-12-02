---
name: Final Project Part 3.1
tools: [Python, HTML, vega-lite, altair]
image: assets/pngs/cars.png
description: This is our final project named 'New York City Leading Death Causes Analysis'. This project contains 3 visualizations analysing 3 different datasets.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

<h1><center>  New York City Death Cause Analysis </center></h1>

#### Primary Visual: New York City Average Death analysis based on Race Ethnicity and Sex




<vegachart schema-url="{{ site.baseurl }}/assets/json/race_ethnicity_deathsNYC.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/_data/New_York_City_Leading_Causes_of_Death.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

