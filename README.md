# Climate Change Modeling 

This project predicts and visualizes **temperature anomalies** using historical environmental data. It combines data science, machine learning, and interactive visualizations to model climate trends from **1961 to 2035**.

---

## 📌 Project Objective

To develop a machine learning model that can forecast **temperature anomalies** (deviations from average global temperature) based on historical environmental records. The predictions help in understanding the **impact of global warming** and support climate awareness and planning.

---

## 📊 Dataset Overview

- **Source:** FAO (Food and Agriculture Organization)
- **File Used:** `Environment_Temperature_change_E_All_Data_NOFLAG.csv`
- **Time Period:** 1961–2019 (historical data)
- **Target Feature:** `Temperature change` per country per year
- **Forecast Range:** 2020–2035

---

## ⚙️ Tech Stack

| Tool         | Purpose                          |
|--------------|----------------------------------|
| Python        | Programming Language              |
| Pandas        | Data manipulation & cleaning     |
| Seaborn/Matplotlib | Data visualization         |
| XGBoost       | Machine learning model (regression) |
| Scikit-learn  | Metrics and preprocessing        |
| Streamlit     | Web-based visualization app      |

---

## 🧠 Model Used

**XGBoost Regressor** was chosen for its:
- Excellent performance on tabular time series data
- Built-in regularization to prevent overfitting
- Ability to capture non-linear patterns in climate trends

---

## 📈 Workflow Summary

1. **Data Preprocessing**
   - Filtered temperature anomaly data by country
   - Averaged values across months for each year
   - Cleaned and reshaped into a structured format

2. **Model Training**
   - X = Year, y = Temperature Anomaly
   - Trained using XGBoost Regressor
   - Evaluated with metrics like MAE, MSE, and R²

3. **Forecasting**
   - Predicted temperature anomalies from 2020 to 2035
   - Combined historic + future data for trend analysis

4. **Visualization**
   - Line plots, bar charts, trendlines, and cumulative graphs
   - Displayed via Matplotlib/Seaborn in notebook
   - Optionally deployed with Streamlit for interactive use

---

## 📉 Evaluation Metrics

| Metric | Description                  |
|--------|------------------------------|
| MAE    | Measures average error       |
| MSE    | Emphasizes larger errors     |
| R²     | Goodness-of-fit of the model |

> XGBoost achieved high accuracy with a strong R² score and low MAE/MSE, indicating reliable forecasting ability.

---

## 📊 Key Visualizations

- **Historic vs Forecasted Line Plot**  
- **Year-wise Forecast Bar Graph**  
- **Cumulative Anomaly Trendline**  
- **Residual Error Plot (optional)**  
- **Interactive Streamlit App (Optional Dashboard)**

---

## 🚀 How to Run the Notebook

1. Clone/download the project folder
2. Ensure the dataset file is named exactly:  
   `Environment_Temperature_change_E_All_Data_NOFLAG.csv`
3. Open `ClimateChangeModeling.ipynb` in Jupyter Notebook or VS Code
4. Run all cells to:
   - Train the model
   - Visualize the data
   - Generate forecasts

---

## 🌐 Streamlit Web App

You can also run the interactive dashboard:

```bash
streamlit run app.py
