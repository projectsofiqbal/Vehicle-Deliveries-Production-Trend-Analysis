# Vehicle Deliveries & Production Trend Analysis

An end-to-end data science project analyzing global Tesla production trends, delivery performance, and market dynamics from 2015 to 2025. This project features exploratory data analysis (EDA), data visualizations, and predictive modeling using Machine Learning.

---

## 📊 Dataset Overview
The analysis is based on a comprehensive dataset tracking 2,640 records of regional Tesla metrics across 16 dimensions. 

* **Timeline:** 2015 – 2025
* **Regions Covered:** Asia, Europe, Middle East, North America
* **Models Included:** Model S, Model X, Model 3, Model Y, Cybertruck
* **Key Features:** Estimated Deliveries, Production Units, Average Price (USD), Battery Capacity (kWh), Range (km), CO2 Saved (tons), and Charging Stations available.

---

## 📈 Key Analysis & Features

### 1. Data Engineering & Feature Creation
* **Production Efficiency:** Calculated as `(Estimated_Deliveries / Production_Units) * 100` to measure supply chain and inventory utilization.
* **Technical Metrics:** Engineered `Price_per_kWh` and `Range_Efficiency` to track EV performance evolutions over the decade.
* **Time-Series Alignment:** Reconstructed tabular periods into synchronized datetime objects for seamless trend plotting.

### 2. Exploratory Data Analysis (EDA)
* **Outlier Detection:** Utilized Interquartile Range (IQR) analysis and boxplots to isolate exceptional production and delivery months.
* **Statistical Deep Dives:** Examinated market share distributions, regional infrastructure correlation matrices, and vehicle pricing structures across models.

### 3. Machine Learning Models
Two separate **Random Forest Regressor** models were developed to extract predictive insights:

* **Delivery Predictor:** Predicts `Estimated_Deliveries` using vehicle specifications, production units, and structural efficiencies.
    * **Performance:** Achieved an **$R^2$ Score of 99.85%** and a Root Mean Squared Error (RMSE) of ~149 units.
* **Price Predictor:** Evaluates `Avg_Price_USD` dynamics. Enhanced by implementing One-Hot Encoding (`pd.get_dummies`) to capture the weight of categorical variables like `Model` and `Region`.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebooks
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (`RandomForestRegressor`, `train_test_split`, metrics evaluation)

---

## 🚀 How to Run the Notebook
1. Clone this repository:
   ```bash
   git clone [https://github.com/projectsofiqbal/Vehicle-Deliveries-Production-Trend-Analysis.git](https://github.com/projectsofiqbal/Vehicle-Deliveries-Production-Trend-Analysis.git)
