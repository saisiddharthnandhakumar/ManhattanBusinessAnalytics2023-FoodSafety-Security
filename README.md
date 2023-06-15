# Manhattan Business Analytics Competition 2023
This project was done for the Manhattan Business Analytics Competition 2023. The topic was to develop a model to analyze Food Security/Safety in Sub-Saharan Africa and Central America/Caribbean Islands. The team who accomplished this and won the best poster award was me(Saisiddharth Nandhakumar), Emily Richey, Andrew Le, and Naomi Raeford from the College of Business at Nicholls State University.

## Tech Stack
Programming Languages: Python, R

Tools: Tableau, Microsoft Excel, Microsoft Powerpoint, Jupyter Lab, R Studio

## Data Collection
The datasets we were suggested from the FAO (Food and Agricultural Organization) from where we got variables about Food Security which was our dependent variable, agricultural production, trade variables like the import and export of different types of fruits, vegetables, grains, etc. 
We also got some variables from the World Bank such as population, Gross Domestic Product (GDP), labor participation rate, and average precipitation. 

Totally we had over 147 variables from the years 1970 to 2022.

In addition to these widely available datasets, we also conducted interviews with Africans who have migrated to the US over the years to gain an insider's scoop on what their take was on the situation of food security in Africa. This was also to check if there was any bias in the data, which we did find.

Example raw data is in Capital_Stock_2.csv

![FAO_logo_Blue_2lines_en_0](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/assets/79336332/8e758369-13c6-4436-ae4b-4a0568e9fbf5)

## Data Cleaning
Most of the cleaning and transformations were done using Python.
As you can see below, we had to remove a lot of columns and filter out the type of observations we needed.

![image](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/assets/79336332/98db2882-2b4c-4303-96ea-58d22bd23175)
To convert it into this, (wide to long format) (suitable for time series analysis)

![image](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/assets/79336332/0d62ca2a-fc06-4ec3-bf03-bcfbb57f01b6)

## Data Preparation
Out of 343,795 cells of data, 233,904 cells were missing. To further elaborate, there was a lot of missing data for many countries and many years as well. This is possibly due to the lack of digital infrastructure in many of the Sub-Saharan countries. We used data from other reliable sources like the World Bank to replace the missing data.

We created many additional calculated columns (feature engineered) like GDP per capita by dividing GDP by the population and dummy coded variables like for if a country was 'coastal' or 'inland'.
