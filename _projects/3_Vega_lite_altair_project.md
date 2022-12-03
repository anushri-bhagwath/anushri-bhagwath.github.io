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
<h6><center><i> Group 7: Members - Anushri Bhagwath & Srushti Karangale </i></center></h6>
<br>
<p align="justify">In this project we are analysing the different causes of deaths that have occurred in New York City between the years 2010 to 2015.</p>

#### <b> Main Dashboard : New York City Average Death analysis based on Race Ethnicity and Sex</b>
<br>
<p align="justify">The main dataset tells us about the different leading causes of death in the city of New York between the years 2007 to 2019 according to sex and ethnicity. It is mentioned in the link (https://catalog.data.gov/dataset/new-york-city-leading-causes-of-death) that the causes of death is obtained from the death certificates of the deceased people which is issued after every death in the city of New York. The metadata is updated as per the latest date.
For our visual, we have created a dashboard which uses a subset of the main dataset and analyses the deaths in New York City between the years 2010 to 2015.</p>
<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/race_ethnicity_deathsNYC2.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 
<div class="left">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/_data/New_York_City_Leading_Causes_of_Death.csv" text="The Data" %}
</div>
<div class="right">
{% include elements/button.html link="https://github.com/anushri-bhagwath/anushri-bhagwath.github.io/blob/main/python_notebooks/bhagwath-anushri-karangale-srushti-FinalProjectPart3.1.ipynb" text="The Analysis" %}
</div>

<br><br>

<p align="justify">The dashboard will provide a comprehensive overview of the average fatalities in New York City from 2010 to 2015 based on race, ethnicity, and sex. The first plot, also known as the "driver" plot, is a straightforward line chart on the dashboard's left side that shows the average number of fatalities in New York City on the y-axis and the race and ethnicity of the deceased on the x-axis. A tooltip containing the average death value for each Race-Ethnicity is displayed when the cursor is hovered over the four critical places on the line graphic for each Race-Ethnicity value. The second plot, often known as the "driven" plot, is a grouped bar chart that shows the average number of fatalities in New York City on the y-axis and the Year data on the x-axis. It is located on the right side of the dashboard. The data on the x-axis are divided into groups based on sex, either male or female. Understanding which color corresponds to which sex is made easier by the legend in the top right corner of the right image. The average annual death values for each sex are displayed when the cursor is above the bars. Selecting a section of the data on the left (driver) visual will enable interaction between the two linked dashboard visuals. Simply doing a left-click on the left visual and sliding the pointer to the right will perform the selection. The visual on the right (driven plot) will alter depending on the area that is picked on the left (driver) visual. As a result, the generated plot on the right side of the screen will show the average annual mortality rate by sex for the selected Race-Ethnic group. 
</p>

<br>
#### <b>Contexual Visuals</b>
<br>
<p align ="justify"> These contextual visualizations will help us learn more about the death causes in New York City. </p>
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

<p align="justify"> The above visual is created using the New York City Community Health Survey dataset. It had various fields which provides us added information such as percentage of people with no access to medical care, access to health insurance, their lifestyle choices such as diet, smoking habits etc. We considered this particular dataset since these factors could provide us extra information to how these lifestyle choices and external factors are also a contributor to the cause of death in NYC. We plotted a simple bar graph for this visualization that shows us the percentage of people without medical care from the years 2011 to 2014. This percentage might include the people from different sex and race ethnicity. Medical negligence can be one of the important causes of deaths in any city.</p>
<br>
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

<p align="justify">For the second contextual visualization, we chose to plot a graph of Causes of death vs Average death over the years specifically for New York City by using grouped bar chart. The dataset used for this was NCHS - Leading Causes of Death: United States. This dataset contained the different causes of deaths and the number of deaths that occurred for each cause in every state in the country since 1999. For our visual we filtered the data to create a plot only for the years between 2010 and 2015. It is interesting to see the similarly in the leading causes of death in NYC across the years as the most deaths were caused by heart related conditions in all four years.</p>

<br>