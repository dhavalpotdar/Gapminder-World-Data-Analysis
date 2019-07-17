# Gapminder-World-Data-Analysis

Gapminder has collected a lot of information about how people live their lives in different countries, tracked across the years,
and on a number of different indicators. The Gapminder Foundation is a non-profit venture registered in Stockholm, Sweden, that promotes sustainable global development and achievement of the United Nations Millennium Development Goals by increased use and understanding of statistics and other information about social, economic and environmental development at local, national and global levels.

This repo looks into how the world has changed across these indicators to answer some interesting questions. The analysis process addresses data quality and tidiness issues and goes through, step by step to produce Explanatory Visualizations that answer the questions raised, as the end result.

# Data 

The data used can be downloaded from Gapminder [here.](http://www.gapminder.org/data/)

Following are the indicators analyzed:
- **Literacy Rate** <br>
The percentage of people ages 15 and above who can, with understanding read and write a short, simple statement on their everyday life.
- **GDP Per Capita** <br>
Gross Domestic Product per person adjusted for differences in purchasing power (in international dollars, fixed 2011 PPP based on 2011 ICP). 
- **Life Expectancy** <br>
The average number of years a new born child would live if current mortality patterns were to stay the same.
- **Employment Rate** <br>
Percentage of total population, age group 15-24, that has been employed during the given year.
- **Forest Coverage** <br>
Percentage of total area that has been covered with forest during the given year; excluding the wooded land, which is spanning more than 0.5 hectares, with trees higher than 5 meters and a canopy of 5-10 percent, or trees able to reach these threshold in situ, or with a combined cover of shrubs, bushes and trees above 10 percent. 
- **Human Development Index** <br>
Human Development Index is an index used to rank countries by level of "human development". It contains three dimensions: health level, educational level and living standard. 
- **Population Density** <br>
Average number of people on each square km of land in the given country. 

# Analysis
The Analysis Process has been carried out with documentation in two Jupyter Notebooks which can be downloaded from the repo or previewed here:
- Data Preparation: `cleaning_act.ipynb` | [Preview](https://nbviewer.jupyter.org/github/dhavalpotdar/Gapminder-World-Data-Analysis/blob/master/cleaning_act.ipynb)
- Exploratory Data Anaysis: `analyzing_act.ipynb` | [Preview](https://nbviewer.jupyter.org/github/dhavalpotdar/Gapminder-World-Data-Analysis/blob/master/analyzing_act.ipynb)

# Conclusion
The following conclusions were made from the analysis:
- Certain metrics like __Literacy Rate, GDP Per Capita, Life Expectancy Years, Human Development Index and Population Density__ show a consistently __increasing trend__ while others such as __Youth Employment Rate (Age: 15 - 24), Percentage Forest Cover__ have been __decreasing__. Percentage Forest Cover decreased sharply in the early 90's and has been decreasing steadily ever since. <br> The decrease in Youth Employment Rate could be explained by an increasing number of students aged 15 to 20 opting for higher education. However, further investigation is needed to ascertain this.


- A brief comparison of Literacy Rates showed that countries __Hungary, Moldova, and Italy share the highest literacy rate__ ever recorded during the __range 1991 - 2011__; while countries like __Niger, Burkina Faso, Guinea and Mali lie at the bottom end__ of the spectrum. There may be other countries having higher or lower rates which were not highlighted by the dataset due to a large number of missing values.


- There exists a __weak negative correlation__ (r = -0.12) between __Percentage Forest Cover__ and __Population Density__. Although the correlation isn't strong, on the global scale, it could still be significant. However, since correlation does not imply causation, further research is required to say deterministically whether an increase in population density causes forest cover to decrease.


- It was found that __Human Development Index strongly correlates with Life Expectancy at Birth__ (r = 0.85). For countries that have HDI = 0.8 and above, its highly likely that their Life Expectancy will be at least 67 years.


- Other than HDI, __GDP Per Capita also influences Life Expectancy__. Countries with high HDI and GDP Per Capita tended to have high life expectancy; while those with lower values, tended to have a lower Life Expectancy at Birth.
