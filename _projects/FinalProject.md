---
name: Global Perspectives -- Mapping the Journey of International Students in US Institutions
tools: [Python, HTML, vega-lite]
image: assets/pngs/cover_World.png
description:
  - "Authors: Wanheng Li & Xiao Zeng"
  - "Data Credit: opendoorsdata.org"
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


### Authors: Wanheng Li & Xiao Zeng


Welcome to our Global Perspectives: Mapping the Journey of International Students in the United States! This is an interactive website that delves into the dynamics of international study in the United States. Through three comprehensive visualizations, we showcase study trends from 1949 to 2023 on a global scale, a country-level perspective, and an institutional viewpoint. This resource serves as an information-rich study database and provides the latest study insights for the academic year 2022-2023.




## Line Chart - Trends in Enrollment of International Students in the U.S.:


<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz1.json" style="width: 100%"></vegachart>


<small>Institute of International Education (2023). "International Student Totals by Place of Origin, 2000/01-2022/23." Open Doors Report on International Educational Exchange.</small>




This line chart depicts the trends in the number of international students originating from different continents/superregions, dating back to 1949. A dropdown menu provides the option to choose a specific continent/superregion, enabling the display of all countries within the selected area. This chart offers detailed insights into how the attractiveness of U.S. institutions to global students has evolved over time. 






## World Map - Global Student Origins:


<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz2.json" style="width: 100%"></vegachart>


<small>Duncalfe, Luke (2022). "ISO-3166-Countries-with-Regional-Codes." Github.</small>




This map features the origins of international students on an interactive 
world map. Countries on the map are color-coded based on the number of international students from that country in the 2022/23 academic year, with deeper shades indicating a higher student count. Hovering the mouse over a country will reveal its name and the count of its international students enrolled in U.S. institutions for the 2022/23 academic year. Selecting a country by clicking on it will generate a line chart showing the trends in student numbers from that country over the years. Multiple countries can be selected to compare their trends. Selection can be reset to the default state by double-clicking on an empty space.






## U.S. State Map - States Hosting International Students & Top 25 Leading Institutions:


<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz3.json" style="width: 100%"></vegachart>


<small>Institute of International Education (2023). "Leading Institutions Hosting International Students, 2022/23." Open Doors Report on International Educational Exchange. Retrieved from http://www.opendoorsdata.org.</small>


<small>Institute of International Education (2023). "Leading Hosts Institutions, 2022/23." Open Doors Report on International Educational Exchange. Retrieved from http://www.opendoorsdata.org. </small>




This visualization seamlessly integrates a U.S. map with a bar chart, presenting a comprehensive overview of international student enrollment across various states. States are color-coded on the map, with darker shades indicating higher numbers of international students and lighter shades representing lower enrollment. The visualization aims to assist in identifying states that are particularly popular or less favored among international students.
Furthermore, the U.S. map features points which highlight the top 25 institutions that attracted the most international students from 2022 to 2023. Notable institutions such as New York University, Northeastern University Boston, and Columbia University stand out in this period. Leveraging interactive features, feel free to click or hold down “Shift” to select multiple points, and explore the scale of international students at these leading institutions.
On the flip side, exploration of the geographical locations of institutions is achievable by selecting the corresponding bars in the bar chart. This dual approach offers a versatile method for examining not only the general distribution of international students across states but also the specific number of international students in these leading institutions.






Through this visualization platform, you can gain a comprehensive understanding of U.S. study dynamics. Our charts not only provide profound insights but also allow you to delve into specific data points of interest through interactivity. Whether you're a scholar, decision-maker interested in study trends, or a student planning to study abroad, this platform offers valuable information and inspiration. Explore the opportunities in international education and embark on your study journey!




### Color Schemes for Viz:
Colors are chosen to enhance the clarity and effectiveness of information presentation. For Viz 1, each continent/superregion and country is coded with a distinct color for differentiation. Upon selecting a continent or superregion, other lines will fade to gray, emphasizing the chosen selection.


For Viz 2, Viridis, a popular continuous color scheme, is selected to ensure smooth and gradual transitions in color coding for the countries.Additionally,it aims to be friendly to individuals with color vision deficiencies. 
As for Viz 3, which focused on the United States, a red color scheme is chosen for differentiation. This will  create a visual contrast between the world map and the U.S. map. Additionally, different intensities of red are employed to emphasize the varying ranges of international students in each state. The bar chart utilizes a contrasting green color scheme for visual comparison.






### Data Analysis
[**Python Notebook**](https://github.com/WanhengL/WanhengL.github.io/blob/main/python_notebooks/International%20Students%20in%20the%20US%20analysis.ipynb)




### Data Link:
##### Main Viz Data Link


1. [**All Places of Origin**](https://opendoorsdata.org/data/international-students/all-places-of-origin/)


##### Contextual Viz Data Link


1. [**ISO country code**](https://github.com/lukes/ISO-3166-Countries-with-Regional-Codes/blob/master/all/all.csv)


2. [**Leading Institutions**](https://opendoorsdata.org/data/international-students/leading-institutions/)


3. [**Hosting International Students**](https://opendoorsdata.org/infographic/u-s-states-hosting-international-students-2022-23/)







<!-- these are written in a combo of html and liquid -->


<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>





