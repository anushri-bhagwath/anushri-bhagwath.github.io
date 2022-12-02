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

<h1><center><b>  New York City Death Cause Analysis </b></center></h1>

<br>
### Primary Visual: New York City Average Death analysis based on Race Ethnicity and Sex
<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/race_ethnicity_deathsNYC.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 
<div class="left">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/_data/New_York_City_Leading_Causes_of_Death.csv" text="The Data" %}
</div>
<div class="right">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/python_notebooks/bhagwath-anushri-karangale-srushti-FinalProjectPart3.1.ipynb" text="The Analysis" %}
</div>

<br><br>

### Contexual Visuals
<br>
#### 1. Percentage of patients without proper medical care over the years in New York City

<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/percent_without_medical_care.json" style="width: 100%; text-align:center" ></vegachart>

<!-- these are written in a combo of html and liquid --> 
<div class="left">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/_data/New_York_City_Community_Health_Survey.csv" text="The Data" %}
</div>
<div class="right">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/python_notebooks/bhagwath-anushri-karangale-srushti-Final-Project-contextual1.ipynb" text="The Analysis" %}
</div>

<br><br>

#### 2. Causes of Death vs Average Deaths over the years in New York City

<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/death_causes.json" style="width: 100%; text-align:center" ></vegachart>

<!-- these are written in a combo of html and liquid --> 
<div class="left">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/_data/NCHS_-_Leading_Causes_of_Death__United_States.csv" text="The Data" %}
</div>
<div class="right">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/python_notebooks/bhagwath-anushri-karangale-srushti-Final-Project-contextual2.ipynb" text="The Analysis" %}
</div>

<br><br>
