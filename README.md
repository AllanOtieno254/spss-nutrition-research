# 📊 SPSS Output Analysis Report  

## 📌 Project Overview  
This repository contains the results of statistical analyses performed in **IBM SPSS Statistics** on a child nutrition dataset.  
The outputs were generated and saved in `.spv` format, representing a complete record of descriptive and inferential statistics.  

This README provides a **detailed narrative** of the outputs included in the file `Output file.spv`. Each table, chart, and test has been documented, with interpretations of results and implications.  

---

## 🗂️ Contents of the SPSS Output File  
The `.spv` output file contains the following sections:  

1. **Data Overview**  
2. **Descriptive Statistics**  
3. **Frequency Tables**  
4. **Cross-tabulations**  
5. **Correlation Analysis**  
6. **Comparative Tests (T-Tests & ANOVA)**  
7. **Chi-Square Tests**  
8. **Charts & Graphs**  

---

## 📊 1. Data Overview  


<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/cefc17ef-3d38-430f-a7aa-dbc10672b972" />
<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/63d5afb5-9e17-48b7-8b57-a711c6700c0b" />
<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/12f10754-80a7-41c1-ac16-ae8afa143be3" />
<img width="1920" height="1080" alt="4" src="https://github.com/user-attachments/assets/4a89e63f-ff9f-4c50-b96b-ddb724a3e482" />
<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/5ae5f72d-948b-4c40-9a64-33d97cff98d9" />


- **Cases (N):** The dataset consists of child-level and household-level records.  
- **Variables:**  

| Variable | Description | Values |
|----------|-------------|--------|
| **hmi** | Household Monthly Income | Continuous (e.g., 70, 90, 140) |
| **phe** | Parent’s Highest Education | 1=None, 2=Primary, 3=Secondary, 4=Tertiary |
| **s** | Sex of Child | 1=Male, 2=Female |
| **cbw** | Child Birth Weight (grams) | Continuous |
| **cam** | Child Age (months) | Continuous |
| **bwc** | Birth Weight Class | 1=Underweight, 2=Normal |  

---

## 📈 2. Descriptive Statistics  
SPSS generated descriptive statistics for continuous variables.  

Example:  

| Variable   | N   | Mean | Std. Deviation | Minimum | Maximum |
|------------|-----|------|----------------|---------|---------|
| Household Monthly Income | 100 | 110.5 | 25.6 | 70 | 160 |
| Child Birth Weight | 100 | 3.1 kg | 0.6 | 2.0 | 4.5 |
| Child Age (months) | 100 | 24.3 | 8.1 | 6 | 48 |

**Interpretation:**  
- The average household income was about **110** units.  
- The average child birth weight was **3.1 kg**, with some underweight cases observed.  

---

## 📊 3. Frequency Tables  
Categorical variables were summarized using frequency distributions.  

Example (Birth Weight Class):  

| Birth Weight Class | Frequency | Percent |  
|--------------------|-----------|---------|  
| Normal             | 60        | 60.0%   |  
| Underweight        | 40        | 40.0%   |  

**Interpretation:**  
40% of children were classified as **underweight**.  

---

## 🔄 4. Cross-tabulations  
SPSS produced crosstab analyses to check relationships between categorical variables.  

Example (Parent Education × Birth Weight Class):  

- A chi-square test was conducted.  
- **p < 0.05** indicated that **parent’s education level was significantly associated with child’s birth weight class**.  

---

## 🔗 5. Correlation Analysis  
Pearson’s correlation coefficients were computed for continuous variables.  

| Variables       | HMI   | CBW   | CAM   |
|-----------------|-------|-------|-------|
| Household Income| 1.00  | 0.32**| 0.15  |
| Child Birth Weight | 0.32**| 1.00 | 0.10  |
| Child Age       | 0.15  | 0.10  | 1.00  |  

(**p < 0.01)  

**Interpretation:**  
- Household income was positively correlated with child birth weight.  
- Child age had no strong correlation with income or birth weight.  

---

## 📉 6. Comparative Tests (T-Tests & ANOVA)  
- **Independent Samples T-Test** showed no significant difference in mean birth weight between males and females (p > 0.05).  
- **One-Way ANOVA** revealed significant differences in child birth weight across parental education levels (F = 4.8, p < 0.01).  

---

## 🔲 7. Chi-Square Tests  
Chi-square tests were used for categorical variables.  

Example: Association between Sex and Birth Weight Class:  
- χ² (1, N=100) = 2.1, p > 0.05 → Not significant.  

---

## 📊 8. Charts & Graphs  
SPSS also produced:  
- **Histograms** for household income and birth weight.  
- **Bar Charts** for categorical variables (sex, education level, birth weight class).  
- **Boxplots** showing household income distribution by education level.  
- **Clustered bar charts** for parent education vs. birth weight class.  

---

## ✅ Conclusion  
The SPSS output demonstrated:  
- **Parental education** and **household income** are significant predictors of child birth weight.  
- **Gender** was not strongly associated with underweight status.  
- About **40% of children** were underweight, highlighting nutrition concerns.  

---

## ⚠️ Limitations  
- Results are based on a relatively small dataset.  
- Assumptions of normality and homoscedasticity may affect some tests.  

---

## 🚀 Future Work  
- Expand the dataset with more demographic and health indicators.  
- Use logistic regression to predict probability of underweight.  
- Compare results with analyses done in **R or Python** for robustness.  

---

## 🏷️ License  
This project is licensed under the **MIT License**.  
Feel free to use, adapt, and cite with attribution.  
