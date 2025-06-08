# 🚴‍♂️ Bike Traffic Forecasting using Machine Learning

This project focuses on forecasting bike traffic using historical data collected at multiple stations. It leverages data preprocessing, EDA, feature engineering, and ML modeling (XGBoost) to accurately predict bike ride counts.

---

## 📊 Dataset Description

The project uses three datasets:

- **rides_15min.csv**: Bike ride counts recorded every 15 minutes at different stations.
- **rides_day.csv**: Daily aggregated ride data, including weather details.
- **bikestations.csv**: Metadata about the measuring stations.

---

## 🧪 Project Objectives

- Clean and preprocess raw data
- Perform descriptive and visual analysis
- Forecast bike rides using ML models
- Evaluate model performance
- Visualize key insights and feature importances

---

## 🛠️ Tech Stack

- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, XGBoost, Pickle  
- **IDE:** Jupyter Notebook  

---

## 🔄 Workflow

### ✅ Step-by-step Process:

1. **Loading Data**
   - Used `read_csv()`, explored using `.info()`, `.describe()`, and checked for nulls

2. **Data Cleaning & Transformation**
   - Translated column names from German to English
   - Converted date format and dropped redundant date columns

3. **Exploratory Data Analysis**
   - Visualized trends using Seaborn and Matplotlib
   - Identified skewed features

4. **Feature Engineering**
   - Removed multicollinearity (VIF)
   - Encoded categorical variables
   - Dropped unnecessary object columns

5. **Data Scaling & Splitting**
   - Used StandardScaler to normalize features
   - Split into `X` and `Y` for model training

6. **Model Selection & Training**
   - Chose **XGBoost Regressor**
   - Trained models for both daily and 15-min data
   - Compared actual vs predicted values

7. **Model Evaluation**
   - Metrics: MAE, MSE, R²
   - Accuracy:
     - `rides_day`: **~93%**
     - `rides_15min`: **~74%**

8. **Model Interpretation**
   - Visualized feature importance

9. **Model Deployment**
   - Saved using `pickle`
   - Loaded for predictions with test data

---

## 📸 Results

### rides_day.csv

![rides_day.csv](https://github.com/Hameedalahr/Bike_Traffic_Forecasting/blob/main/rides_day.csv%20result.png?raw=true)

### rides_15min.csv

![rides_15min.csv](https://github.com/Hameedalahr/Bike_Traffic_Forecasting/blob/main/ride_15min.csv%20result.png?raw=true)



---

## 📚 Future Improvements

- Use deep learning (e.g., LSTM) for improved time-series forecasting
- Aggregating rides_15min.csv with existing datasets
- Deploy as a web app using Streamlit or Flask

---

## 🙋‍♂️ Author

**Abdul Hameed Syed**  
Data Science Enthusiast 

## For

**LPDG India**


