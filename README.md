# Housing-Market-Analysis

# Housing Market Analysis (Project 3)

This project analyzes how U.S. housing prices, rental prices, college tuition, and the Consumer Price Index (CPI) have changed over the past 25 years. It explores how the cost of living has evolved across major sectors using multiple datasets, including Zillow Home Values, Zillow Rent Index, national college tuition, and CPI. The notebook focuses on comparing trends, computing percent changes, visualizing patterns, and drawing meaningful insights from long-term economic data.


---

## 🎯 Project Goals

- Investigate long-term housing price changes across 3 selected markets  
- Compare housing price growth with rental price growth  
- Compare both with national college tuition and CPI  
- Perform data wrangling, merging, cleaning, and visualization  
- Generate statistical comparisons (correlations, percent changes, trends)  
- Present clear observations, summary, and reflections

---

## 📚 Datasets Used

### **1. Zillow Home Value Index (ZHVI)**
File: `Metro_zhvi_homes_smoothed_2025.csv`  
- Monthly home values for hundreds of US metro areas  
- Smoothed to reduce seasonality  
- You analyze:
  - Raleigh, NC  
  - Greensboro, NC  
  - One additional market of your choice  

### **2. National College Tuition Data**  
File: `college_tuition_data.tsv`  
- Average undergraduate tuition and required fees  
- 1963–present  
- Uses “All institutions, current dollars” column  

### **3. Zillow Observed Rent Index (ZORI)**  
File: `Metro_zori_monthly_rentals_smoothed_2025.csv`  
- Average monthly rent values  
- For the same 3 markets examined in the home price dataset  

### **4. Consumer Price Index (CPI)**  
File: `cpi.csv`  
- Measures inflation from 1913–2024  
- Includes price changes in food, housing, services, transportation, etc.

---

## 🧠 Methods & Workflow

### **1. Data Importing**
- Load CSV/TSV files into DataFrames  
- Inspect dataset structure  
- Convert date columns to usable format  

### **2. Data Wrangling**
- Filter to relevant cities and columns  
- Remove missing values  
- Transpose/pivot where necessary  
- Rename unclear columns  
- Format dates as monthly or annual periods  
- Use groupby to aggregate data (yearly averages, etc.)  
- Merge datasets using year or date index  

### **3. Univariate Analysis**
For each dataset:
- Summary statistics  
- Line plots over time  
- Outlier detection  
- Observations of long-term trends  

### **4. Bivariate Analysis**
Across datasets:
- Compare housing vs. rent  
- Compare housing vs. tuition  
- Compare housing vs. CPI  
- Compare rent vs. tuition  
- Scatter plots, dual-axis plots, correlation tables  

### **5. Percent Change & Rate Comparisons**
- Use `pct_change()` to compute month-to-month changes  
- Convert to *annualized percentage change*  
- Compare:
  - Annual housing growth  
  - Annual rent growth  
  - Annual tuition increases  
  - Annual CPI changes  

---

## 📊 Visualizations

All charts include:
- Accurate titles  
- Labeled axes  
- Legends  
- Proper scaling  
- Multi-series line charts for market comparisons  
- Combined axes when effective  

Common visualizations include:
- Home value trends (3 markets)  
- Rent price trends (3 markets)  
- Tuition growth over time  
- CPI inflation over time  
- Percent change comparisons  
- Correlation heatmaps  

---

## 🔍 Questions Explored

### **Housing Markets**
- How do Raleigh, Greensboro, and your chosen market differ?  
- Which grew the fastest?  
- Were there notable spikes (e.g., 2008 crash, 2020–2022 pandemic boom)?  
- Are there outliers worth explaining?  

### **Tuition vs. Housing**
- Is tuition rising faster than home prices?  
- Are there strong correlation patterns?  
- Are increases consistent or volatile over time?  

### **Rent vs. Housing**
- Do rent and home values move together?  
- Are rent increases lagging or leading housing increases?  

### **CPI vs. Housing**
- Has inflation risen at the same pace as home values?  
- Do major inflation periods align with housing market surges?  

---

## 📝 Summary of Observations (Example)

- Home prices increased dramatically in all markets since 2000  
- Rent has increased but more gradually than housing  
- Tuition rose the fastest over long periods, outpacing CPI and housing  
- CPI shows steady but modest increases compared to tuition/housing  
- Certain markets exhibit sharper booms (e.g., Sun Belt or West Coast cities)  
- Housing and rent are strongly correlated; tuition is not  
- CPI has a weak relationship with tuition but moderate correlation with home prices  

*(Your exact observations go here — these are illustrative placeholders.)*

---

## 🙋 Reflection (Example)

**What I learned**
- How to merge multiple time-series datasets  
- How to wrangle messy real-world data  
- How to compute and interpret percent changes  
- How to create effective visual comparisons  

**Challenges**
- Aligning datasets with different date formats  
- Handling missing or inconsistent years  
- Scaling plots for datasets with vastly different magnitudes  

**What didn’t work**
- Some markets lacked complete rental data  
- Some combined plots were too busy and needed redesign  

---

## 🛠️ Tools & Libraries

Only the allowed packages were used:
- `pandas`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `datetime`
- `warnings` (optional)

---

## ▶️ Running the Project

1. Open `project3.ipynb`  
2. Run all cells from top to bottom  
3. All plots and analysis will appear inline  
4. Ensure the dataset files are in the same directory  

---

## ✔️ Deliverables

- A clean, well-organized Jupyter notebook containing:
  - Dataset descriptions  
  - Data wrangling  
  - Analysis  
  - Visualizations  
  - Summary  
  - Reflections  

---

