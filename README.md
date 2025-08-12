# 🏃 Predictors of Ohio High School Cross Country Success

## 📌 Overview
The goal of this project was to determine the top predictors of Ohio high school cross country running success, considering demographics such as high school enrollment size, 
socioeconomic status, and population density. Through this predictive analysis, we reveal to Ohio high school cross country coaches on how they can make their program more competitive, and
to OHSAA (Ohio High School Athletic Association) on how they can make cross country competition more fair. 

## 📊 Data 
- **Source:** Data includes 2021 high school enrollment data from the [Ohio Department of Education](https://education.ohio.gov/Topics/Data/Frequently-Requested-Data/Enrollment-Data), demographic estimates from the [US Census](https://data.census.gov/), 
state meet results from [OHSAA](https://www.ohsaa.org/sports/cc/pastresults), and district as well as regional meet results from [Baum's Page](https://www.baumspage.com/cc/index.php).
- **Description:** The Ohio Department of Education data includes variables such as `DIST_IRN`, `DIST_NAME`, `BLDG_IRN`, `BLDG_NAME`, and `PRESCHOOL` to `GRADE_12` (enrollment sizes). The census data contained variables with five year estimates on median income, population density, and racial makeup in each Ohio school district from 2020.
The OHSAA and Baum's Page data included variables on team meet results such as `Place`,`Team`,`Gender`, and `Division` in addition to a variable signifying the type of meet (district, regional, state).
- **Target:** The main outcome variables involved in our analysis is all the variables included in the OHSAA and Baum's Page data.
- **Size:** Ohio Department of Education data was approximately 3000 rows and 20 columns. The census data was about 600 rows and 2-100 columns. The cross country performance data was about 10-30 rows and 5 columns.

## 🛠️ Methods
- **Data Gathering, Preprocessing, and Coalescing:** Webscraping (Python, dealing with missing values (Python), manipulating data to be tidy (Python), combining XC performance data with high school enrollment data with string similarity algorithm linking teams to high schools (Python), combining data via SQL
- **Exploratory Data Analysis:** Bar charts
- **Statistical Analysis:** Scatterplots and correlation coefficients, Comparative Boxplots

## 📈 Results
- In Division I, high schools with larger enrollment sizes and in areas with greater household income tend to perform better in cross country. This relationship is not as strong in
Divisions II and III.
- Ohio high school cross country teams in suburban locations show better success. Teams in dense urban areas demonstrate the least success.
- Ohio high school cross country teams in areas with lower poverty levels show higher performance.
- Divison I Ohio high school cross country teams are primarily in suburban and urban areas. Division II and III cross country teams are primarily in small town and rural areas respectively.

## 📌 Future Work
Potential next steps:
- Compare the top predictors of cross country success in Ohio to top predictors of XC success in other states
- Determine how the diversity of landforms around a given high school contributes to cross country success, utilizing data in GIS
- Look at specific case studies of cross country teams at high schools with small enrollment sizes that have won the state meet 
