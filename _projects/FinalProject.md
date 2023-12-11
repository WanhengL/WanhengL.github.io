---
name: Global Perspectives -- Mapping the Journey of International Students in the US 
tools: [Python, Vega-Altair, HTML]
image: assets/pngs/world_map.png
description: 
  - "Authors: Wanheng Li & Xiao Zeng<br>Data Credit: opendoorsdata.org"
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

## Gloval Perspective - Mapping the Journey of International Students in US Institutions
##### Authors: Wanheng Li & Xiao Zeng 


Welcome to our Global Perspectives: Mapping the Journey of International Students in the United States! This is an interactive website that delves into the dynamics of international study in the United States. Through three comprehensive visualizations, we showcase study trends from 1949 to 2023 on a global scale, a country-level perspective, and an institutional viewpoint. This resource serves as an information-rich study database and provides the latest study insights for the academic year 2022-2023.



### Line Chart - Trends in Enrollment of International Students in the U.S.:

<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz1.json" style="width: 100%"></vegachart>
<small>Institute of International Education (2023). "International Student Totals by Place of Origin, 2000/01-2022/23." Open Doors Report on International Educational Exchange.</small>


This line chart depicts the trends in the number of international students originating from different continents or major geographic regions, dating back to 1949. A dropdown menu provides the option to choose a specific continent/region, enabling the display of all countries within the selected area. This chart offers detailed insights into how the attractiveness of U.S. institutions to global students has evolved over time.




### World Map - Global Student Origins:

<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz2.json" style="width: 100%"></vegachart>
<small>Duncalfe, Luke (2022). "ISO-3166-Countries-with-Regional-Codes." Github.</small>


This map features the origins of international students on an interactive 
world map. Countries on the map are color-coded based on the number of international students from that country in the 2022/23 academic year, with deeper shades indicating a higher student count. Hovering the mouse over a country will reveal its name and the count of its international students enrolled in U.S. institutions for the 2022/23 academic year. Selecting a country by clicking on it will generate a line chart showing the trends in student numbers from that country over the years. Multiple countries can be selected to compare their trends. Selection can be reset to the default state by double-clicking on an empty space.




### U.S. State Map - States Hosting International Students & Top 25 Leading Institutions:

<vegachart schema-url="{{ site.baseurl }}/assets/json/Viz3.json" style="width: 100%"></vegachart>


<small>Institute of International Education (2023). "Leading Institutions Hosting International Students, 2022/23." Open Doors Report on International Educational Exchange. Retrieved from http://www.opendoorsdata.org.</small>

<small>Institute of International Education (2023). "Leading Hosts Institutions, 2022/23." Open Doors Report on International Educational Exchange. Retrieved from http://www.opendoorsdata.org. </small>


This visualization seamlessly integrates a U.S. map with a bar chart, presenting a comprehensive overview of international student enrollment across various states. States are color-coded on the map, with darker shades indicating higher numbers of international students and lighter shades representing lower enrollment. The visualization aims to assist in identifying states that are particularly popular or less favored among international students.

Furthermore, the U.S. map features points which highlight the top 25 institutions that attracted the most international students from 2022 to 2023. Notable institutions such as New York University, Northeastern University Boston, and Columbia University stand out in this period. Leveraging interactive features, feel free to click or hold down “Shift” to select multiple points, and explore the scale of international students at these leading institutions.

On the flip side, exploration of the geographical locations of institutions is achievable by selecting the corresponding bars in the bar chart. This dual approach offers a versatile method for examining not only the general distribution of international students across states but also the specific number of international students in these leading institutions.

<br>

### Conclusion

Through this visualization platform, you can gain a comprehensive understanding of U.S. study dynamics. Our charts not only provide profound insights but also allow you to delve into specific data points of interest through interactivity. Whether you're a scholar, decision-maker interested in study trends, or a student planning to study abroad, this platform offers valuable information and inspiration. Explore the opportunities in international education and embark on your study journey!

<br>

### Color Schemes:
Colors are chosen to enhance the clarity and effectiveness of information presentation. For Viz 1, each continent/superregion and country is coded with a distinct color for differentiation. Upon selecting a continent or superregion, other lines will fade to gray, emphasizing the chosen selection.

For Viz 2, Viridis, a popular continuous color scheme, is selected to ensure smooth and gradual transitions in color coding for the countries.Additionally,it aims to be friendly to individuals with color vision deficiencies. 

As for Viz 3, which focused on the United States, a blue color scheme is chosen to match with other visualizations. Additionally, different intensities of blue are employed to emphasize the varying ranges of international students in each state. The bar chart utilizes a contrasting same color scheme for visual comparison.

<br>

### Data Sources:
##### Main Viz Data Link:

<a href="https://opendoorsdata.org/data/international-students/all-places-of-origin/" target="_blank">All Places of Origin</a>

The primary dataset for our main visualization is sourced from "All Places of Origin," providing comprehensive information about international students. The dataset has a total size of 123.03 KB. After thorough cleaning and processing, the key attributes include:

| Df 1 Attribute        | Data Description                                         | Data Type |
|-----------------------|----------------------------------------------------------|-----------|
| Place of Origin       | Name of Continents                                       | Str       |
| 1949/50               | Number of international students in each country in 1949 | Int       |
| ... ...               | ... ...                                                  | ...       |
| 2022/23               | Number of international students in each country in 2022 | Int       |

| Df 2 Attribute        | Data Description                                         | Data Type |
| Place of Origin       | Name of Countries                                        | Str       |
| 2002/03               | Number of international students in each country in 2002 | Int       |
| ... ...               | ... ...                                                  | ...       |
| 2022/23               | Number of international students in each country in 2022 | Int       |

<br>

##### Contextual Viz Data Link:

<a href="https://opendoorsdata.org/data/international-students/leading-institutions/" target="_blank">1. Leading Hosts Institutions</a>

The data for our first contextual visualization is derived from "Leading Host Institutions," with a dataset size of 46.24 KB. Following data cleaning, the relevant attributes are:

| Attribute             | Data Description                                  | Data Type |
|-----------------------|---------------------------------------------------|-----------|
| Institutes            | Hosting institutions in the USA                   | Str    |
| Lat                   | Latitude of the institutions                      | Float     |
| Long                  | Longitude of the institutions                     | Float     |
| City                  | City location of the institutions                 | Str    |
| State                 | State of the institutions                          | Str    |
| State_Abbreviation    | Abbreviation of States                            | Str    |
| ID                    | State ID                                          | Int       |
| Intl_Students         | Number of international students in each institution | Int       |

<br>

<a href="https://opendoorsdata.org/data/international-students/leading-places-of-origin/" target="_blank">2. Leading Places of Origin</a>

Our second contextual visualization draws data from "Leading Places of Origin," with a dataset size of 31.07 KB. After cleaning, the dataset includes attributes such as:

| Attribute             | Data Description                                  | Data Type |
|-----------------------|---------------------------------------------------|-----------|
| Place of Origin       | Name of Countries                                 | Str       |
| 2022/23               | Number of international students in each country  | Int       |
| Country Code          | Country ID code                                   | Int       |

<br>

<a href="https://opendoorsdata.org/infographic/u-s-states-hosting-international-students-2022-23/" target="_blank">3. Leading Institutions Hosting International Students, 2022/2023</a>

The geographical data for our final contextual visualization originates from "Leading Institutions Hosting International Students, 2022/2023," boasting a dataset size of 697.24 KB. After meticulous data cleaning, the essential attributes are:

| Attribute             | Data Description                                  | Data Type |
|-----------------------|---------------------------------------------------|-----------|
| State                 | State of the institutions                         | Str       |
| range                 | Range of international students in each state     | Str       |

<br>

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://opendoorsdata.org/data/international-students/all-places-of-origin/" text="The Main Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/WanhengL/WanhengL.github.io/blob/main/python_notebooks/International%20Students%20in%20the%20US%20analysis.ipynb" text="The Analysis" %}
</div>
