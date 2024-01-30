# Manhattan Business Analytics Competition 2023
This project was done for the Manhattan Business Analytics Competition 2023. The topic was to develop a model to analyze Food Security/Safety in Sub-Saharan Africa and Central America/Caribbean Islands. The team who accomplished this and won the best poster award was me(Saisiddharth Nandhakumar), Emily Richey, Andrew Le, and Naomi Raeford from the College of Business at Nicholls State University.
### Goal: C

Click link for pdf version: [Nicholls State University_Planting the Seeds of Food Security in Sub-Saharan Africa.pdf](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/files/14091115/Nicholls.State.University_Planting.the.Seeds.of.Food.Security.in.Sub-Saharan.Africa.pdf)

![Screenshot 2024-01-29 184245](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/assets/79336332/ddd9c5f3-b048-4632-bfe9-15170b55b620)

## Tech Stack
Programming Languages: Python, R

Tools: Tableau, Microsoft Excel, Microsoft Powerpoint, Jupyter Lab, R Studio

## Data Collection
The datasets we were suggested from the FAO (Food and Agricultural Organization) from where we got variables about Food Security which was our dependent variable, agricultural production, trade variables like the import and export of different types of fruits, vegetables, grains, etc. 
We also got some variables from the World Bank such as population, Gross Domestic Product (GDP), labor participation rate, and average precipitation. 

We had over 147 variables from the years 1970 to 2022.

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

## Data Analysis
Using the R language, we created a multiple-regression model to analyze the statistical significance between the key variables(as shown below) and food security among the countries in sub-Saharan Africa. 
![Screenshot 2024-01-29 184820](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/assets/79336332/8af1947f-3daa-4766-a858-f2fe7f4aae49)

We also visualized the relationship between country location and food security with a violin plot.
![Screenshot 2024-01-29 202350](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/assets/79336332/e3c5f443-468d-4465-8a4e-5a176475de60)

Using Tableau, we visualized most of the other charts like the Hexmap, Line charts, scatterplot, as well as the geographic map.
![Screenshot 2024-01-29 202922](https://github.com/saisiddharthnandhakumar/ManhattanBusinessAnalytics2023-FoodSafety-Security/assets/79336332/0e269edc-101e-4a9d-8403-8ce31a02e689)
