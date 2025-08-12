# 🏃 Predictors of Ohio High School Cross Country Success

## 📌 Overview
This project identifies the **top predictors of Ohio high school cross country performance** using school enrollment, socioeconomic context, and population density.  
Findings can help **coaches** make programs more competitive and inform **OHSAA** discussions on equitable competition structures.

## 📊 Data
- **Sources:**
  - Ohio Department of Education – 2021 enrollment
  - U.S. Census – 5-year demographic estimates 
  - OHSAA – 2017-2021 State meet results
  - Baum’s Page – 2017-2021 istrict & regional meet results
- **Description:**
  - **Education:** `DIST_IRN`, `DIST_NAME`, `BLDG_IRN`, `BLDG_NAME`, `PRESCHOOL`…`GRADE_12` (enrollment by grade)
  - **Census:** median household income, population density, race/ethnicity (2020 5-year estimates)
  - **XC Results:** `Place`, `Team`, `Gender`, `Division`, and meet type (district/regional/state)
- **Target:** Team performance at district, regional, and state meets (e.g., **placement**).
- **Size (approx.):** Education ≈ 3,000 × 20; Census ≈ 600 × 2–100; XC results ≈ 10–30 × 5 per meet file.

## 🛠️ Methods
- **Data gathering & preprocessing:** Web scraping (Python), missing-value handling, tidy reshaping, filtering relevant columns.
- **Record linkage:** String-similarity matching to join team names to high schools; manual spot checks for high-confidence links.
- **Integration:** SQL joins to merge enrollment, demographics, and meet results.
- **EDA:** Distributions and comparisons (bar charts, boxplots).
- **Statistics:** Correlations and scatterplots; comparative boxplots across divisions/locale types.

## 📈 Results
- **Division I:** Larger enrollments and **higher household income** areas are associated with better team performance; the relationship weakens in **Divisions II–III**.
- **Locale effects:** **Suburban** programs tend to outperform; **dense urban** programs show the lowest performance on average.
- **Socioeconomics:** **Lower poverty** correlates with higher team performance.
- **Division geography:** Division I teams are primarily **suburban/urban**; Division II skew **small town**, Division III **rural**.

## 📌 Future Work
- Compare Ohio predictors with those from **other states** to assess generalizability.
- Incorporate **terrain/landform diversity** via GIS to study training environment effects.
- **Case studies** of small-enrollment schools that won state titles to identify outlier success factors.
