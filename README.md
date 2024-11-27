# Best Representative Polling Units in Istanbul Local Elections

This repository contains the implementation and results of a project aimed at identifying the most representative polling units in Istanbul during the 2014 and 2019 local elections. By analyzing election data, the project determines neighborhoods that closely predict city-wide election outcomes, helping survey companies and researchers improve prediction accuracy with less effort.

---

## **Project Overview**

### **Objective**
The project analyzes Istanbul's local election results to identify polling units (neighborhoods) that most closely reflect the overall election results for the city. The primary goal is to assist:
- **Survey companies**: Optimize their efforts by focusing on key polling units.
- **Political analysts**: Gain insights into dynamic electoral patterns in Istanbul.

### **Why Istanbul?**
- Istanbul is Turkey's largest city, with immense political, economic, and demographic significance.
- It generates nearly one-third of Turkey's GDP, making it a key indicator of national electoral trends.

---

## **Methodology**

### **1. Data Collection**
- Election data from the Supreme Election Council (**YSK**) was extracted for both 2014 and 2019 local elections.
- Data included district-wise breakdowns of registered voters, total votes, valid/invalid votes, and votes for political parties.

### **2. Data Preprocessing**
- The data was cleaned and organized using **Microsoft Excel** and **Python**:
  - Combined district and neighborhood data to avoid duplicates.
  - Handled missing or newly introduced neighborhoods between 2014 and 2019 elections.
  - Unified votes for smaller parties into an "OTHERS" category for simplicity.

### **3. Formula-Based Scoring**
- Two error-margin formulas were applied to measure how closely a neighborhood’s results matched the overall city results:
  - **General Percentage Formula**: Compares neighborhood-level vote percentages with city-wide percentages.
  - **Coefficient-Based Formula**: Weighs party-specific discrepancies by their overall city-wide vote share.

---

## **Results**

### **Findings**
- Sorted Excel files for both 2014 and 2019 elections rank neighborhoods based on their predictive accuracy.
- **Top 3 most representative neighborhoods**:
  1. Ümraniye - Çamlık Mahallesi
  2. Küçükçekmece - Cumhuriyet Mahallesi
  3. Bahçelievler - Soğanlı Mahallesi

### **Insights**
- Neighborhoods from districts like **Ümraniye**, **Küçükçekmece**, and **Pendik** consistently rank highly.
- The findings suggest that monitoring these key neighborhoods can provide robust predictions for future elections.

### **Challenges**
- Neighborhood renamings or reorganizations between 2014 and 2019 caused mismatches.
- Smaller political parties with negligible impact were grouped under "OTHERS," reducing complexity but introducing minor inaccuracies.

---

## **How to Use This Repository**

1. **Data Files**:
   - `data/`: Contains cleaned and sorted Excel files for both 2014 and 2019 elections.
   - Files include neighborhood-level vote percentages and calculated error margins.

2. **Python Scripts**:
   - `scripts/`: Includes Python code for data preprocessing and formula application.
   - Dependencies: Install `pandas` and `numpy` using `pip install pandas numpy`.

3. **Reports**:
   - The final report, including analysis and discussion, is available as a PDF in the `reports/` directory.

---
Future Work
Expand analysis to include socioeconomic data for more detailed insights.
Include additional election years for trend analysis.
Develop a predictive model for upcoming elections using machine learning.
References
Esen, B., & Gumuscu, S. (2019). Killing Competitive Authoritarianism Softly: The 2019 Local Elections in Turkey. South European Society and Politics, 24(3), 317–342. DOI
Supreme Election Council (YSK): Election Results


