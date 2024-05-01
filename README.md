# Intergenerational_Mobility_Project
My Data Analytics senior capstone project on Intergenerational Mobility (IGM).
## 1. Project Summary

Intergenerational mobility (IGM) is a critical measure of societal equality and economic opportunity. This study aimed to conduct segmentation analysis on 153 countries using two variable sets: rank-based mobility measures (rank-based variables) and transition matrix measures (transition variables). Through k-means classification, we identified four clusters for each variable set that showed face-value validation through visualization. However, further mixed-method validation suggested limited discriminatory power of the clusters, hence no further support for our classification models. These results suggest over-reliance on The World Bank’s pre-derived mobility measures and their lack of accuracy. They also suggest a potential  non-monotonic relationship between IGM and inequality, which needs more in-depth examination. Future research should try to derive a specific formal indicator for educational IGM. Segmentation attempts could broaden the current educational scope to include other domains of IGM, considering intersectional topics. 

## 2. Author
Josh Vo (vo_j4@denison.edu)

This project was part of my Data Analytics capstone course at Denison University. 
## 3. Prerequisites
### 3.1. Softwares
- Github
- R version 4.3.3
### 3.2. R packages
- leaps
- dplyr
- ggplot2
- ggforce
- stats
- ggalt
- plot3D
- plotly
- gridExtra
- cluster
- factoextra
- caret

## 4. Data and variables 
#### 4.1. Global Database On Intergenerational Mobility (GDIM; The World Bank, 2023; Van Der Weide et al., 2021)  [Link](https://datacatalog.worldbank.org/search/dataset/0050771/global-database-on-intergenerational-mobility)
The GDIM included summary survey data from 153 countries collected between 1991 and 2017, representing 97% of the world population. It contained evaluations of IGM in education for 10-year cohorts, encompassing individuals born from 1940 to 1989. This dataset had been cleaned and synthesized by its collector.
- Mobility metrics derived from previous report by Van Der Weide et al. (2021):
  - CAT: absolute mobility measure 1
  - YOS: absolute mobility measure 2
  - 1-COR: relative mobility measure 1
  - 1-BETA: relative mobility measure 2
- Rank-based mobility measures: 12 variables that showed the percentage of children who ended up in different quartiles of the education hierarchy, given that their parents were at the bottom half
- Transition measures: 25 variables that showed the movements in educational attainment after one generation on the International Standard Classification of Education (ISCED) scale
- Year of survey collection
#### 4.2. Global Gini Index Data (GGID; The World Bank, 2024). [Link](https://data.worldbank.org/indicator/SI.POV.GINI?)
This dataset contained annual Gini indices of 266 countries from 1963 to 2022 (retrieval date: Feb 28th, 2024)
- Inequality: measured through the Gini index (The World Bank, 2023)
- Year of survey collection
## 5. Documents
- Code file "IGM project - Code file"
- HTMP output for code file "IGM project - Code file.html"
- Paper  [Link](https://docs.google.com/document/d/1yu36w1Ff-UCqprAcB1T-7oHwUTLPF-BXieYC_KsXkBA/edit?usp=sharing)
- Data folder, containing:
  - Data file to make up for Gini NA values "NA gini data"
  - Dataset 1 for Gini index "Gini dataset"
  - Dataset 2 for global IGM data "GDIM dataset"
