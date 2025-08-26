# Literacy Rates Data Analysis

This repository contains the data cleaning, exploration, and visualization of global literacy rates. The analysis was performed using Python, Pandas, Seaborn, and Matplotlib in Google Colab.

---

## Open in Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

---

## Dataset

- **File:** `literacy_rates_updated.csv`  
- **Link:** [Download Dataset](YOUR_DATASET_LINK_HERE)

### Sample Data

| Region                        | Country      | Year | Age   | Gender | Literacy rate |
|-------------------------------|------------|------|-------|--------|---------------|
| Central and Southern Asia     | Afghanistan | 2011 | <15   | female | 0.176121      |
| Central and Southern Asia     | Afghanistan | 2011 | <15   | male   | 0.454171      |
| MISSING                        | Afghanistan | 2011 | 15-24 | female | 0.321132      |
| MISSING                        | Afghanistan | 2011 | 15-24 | male   | 0.618791      |
| Central and Southern Asia     | Afghanistan | 2011 | 25-64 | female | 0.084128      |

---

## Data Cleaning

- **Removed duplicates** to ensure no repeated records.  
- **Handled missing values**:  
  - Missing regions were labeled as `MISSING`.  
  - Missing literacy rates were set to `-1`.  
- **Fixed typos** and inconsistencies in `Year` and `Gender` columns.  
- **Converted data types**: `Year` to integer and `Literacy rate` to float.  
- **Final check** confirmed no duplicates, missing values, or inconsistencies remain.

---

## Data Exploration

### Univariate Analysis

**Region Counts**  
- Latin America and the Caribbean has the highest number of records.  
- Sub-Saharan Africa follows.  
- Oceania and the MISSING category have the fewest records.  

**Year Distribution**  
- Data is unevenly distributed across years.  
- Peaks observed in 2011 and 2018.

---

### Multivariate Analysis

**Literacy Rate by Region**  
- Sub-Saharan Africa has the lowest literacy rate.  
- Europe and Northern America has the highest.

**Literacy Rate by Gender**  
- Both genders show high literacy rates overall.  
- Females have a slightly lower median and wider spread than males.  
- Outliers exist in both genders.

**Literacy Rate by Age and Gender**  
- Males consistently have higher literacy rates than females across all age groups.  
- Literacy peaks in the 15–24 age group.  
- Significant drop observed in the 65+ age group.

---

## Visuals

**Region Count**  
![Region Count](images/region_count.png)

**Year Distribution**  
![Year KDE](images/year_kde.png)

**Literacy Rate by Region**  
![Region Literacy](images/literacy_region.png)

**Literacy Rate by Gender**  
![Gender Literacy](images/literacy_gender.png)

**Literacy Rate by Age and Gender**  
![Age Gender Literacy](images/literacy_age_gender.png)

---

## Summary

- Data cleaning addressed **duplicates, missing values, typos, and incorrect data types**.  
- Univariate plots reveal **distribution across regions and years**.  
- Multivariate plots highlight **differences in literacy by region, gender, and age**.  
- The cleaned dataset is ready for further analysis or modeling.

---

**Libraries Used:**  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

**Dataset:** `literacy_rates_updated.csv`  
**Environment:** Google Colab
