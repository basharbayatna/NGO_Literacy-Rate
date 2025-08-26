# Literacy Rates Data Analysis

This repository contains the data cleaning, exploration, and visualization of global literacy rates. The analysis was performed using Python, Pandas, Seaborn, and Matplotlib in Google Colab.

## Project Context

Your task is to clean and explore data for a **non-profit organization focused on promoting and increasing youth literacy rates**. They are particularly interested in understanding where they should focus their next project and what strategies to use to have the biggest impact in increasing youth literacy rates in that area.  

This analysis aims to provide **insights on literacy rates across regions, genders, and age groups**, helping the organization make data-driven decisions.



---

## Dataset


- **Link:**(https://docs.google.com/spreadsheets/d/1wS3BIjAdGRQHTwGAG5adwj0Mi0Q6HRdKmc05eG4YCmI/edit?gid=1121421486#gid=1121421486)

### Sample Data

| Region                        | Country      | Year | Age   | Gender | Literacy rate |
|-------------------------------|------------|------|-------|--------|---------------|
| Central and Southern Asia     | Afghanistan | 2011 | <15   | female | 0.176121      |
| Central and Southern Asia     | Afghanistan | 2011 | <15   | male   | 0.454171      |
| MISSING                        | Afghanistan | 2011 | 15-24 | female | 0.321132      |
| MISSING                        | Afghanistan | 2011 | 15-24 | male   | 0.618791      |
| Central and Southern Asia     | Afghanistan | 2011 | 25-64 | female | 0.084128      |

---

## Literacy Rate Definition

Literacy rate is calculated as the number of literate persons in a specific age and gender group divided by the total number of persons in that group.  

A person is considered **literate** if they are able to **read and write, with understanding, a short, simple statement about everyday life**.  

Rates at or near **100%** indicate that nearly every individual in that age and gender group is able to read and write at least at a basic level.

---

## Data Cleaning

- **Removed duplicates** to ensure no repeated records.  
- **Handled missing values**:  
  - Missing regions labeled as `MISSING`.  
  - Missing literacy rates set to `-1`.  
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
- Literacy rates provide insight into **the ability of populations to read and write**, with higher values indicating nearly universal literacy in the group.  
- The cleaned dataset is ready for further analysis or modeling.

---

**Libraries Used:**  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  


**Environment:** Google Colab
