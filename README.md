 🌍 Air Quality Prediction & Health Risk Assessment in Bangladesh
📌 Overview

This project aims to **predict Air Quality Index (AQI)** and classify pollution levels across districts of Bangladesh using **Machine Learning**.
The system leverages **pollutant data** (PM2.5, PM10, O₃, NO₂, SO₂, CO), **weather data** (temperature, humidity, wind speed, rainfall, pressure, clouds), and **location data** (district, division, coordinates).


🎯 Objectives

* Predict **future AQI values** (Regression)
* Classify AQI into **pollution categories** (Good, Moderate, Unhealthy, Hazardous)
* Identify **key factors influencing air quality**
* Provide a **dashboard** for health risk alerts

 🛠 Technologies Used

* **Python 3**
* **Pandas, NumPy** → Data handling
* **Matplotlib, Seaborn** → Data visualization
* **Scikit-learn** → ML models (Regression & Classification)
* **XGBoost** → Advanced prediction
* **Streamlit** → Interactive dashboard

---

 📂 Project Structure

```
📁 Air-Quality-Prediction
│── 📄 dataset.csv              # Original dataset (weather + pollutants)
│── 📄 preprocessing.py         # Data cleaning & feature engineering
│── 📄 eda.ipynb                # Exploratory Data Analysis (EDA)
│── 📄 regression_model.py      # AQI prediction (regression models)
│── 📄 classification_model.py  # AQI category prediction (classification)
│── 📄 evaluation.py            # Model metrics & feature importance
│── 📄 README.md                # Project documentation


📊 Methodology

1. **Data Preprocessing**

   * Convert `date` → `month`
   * Encode categorical (`district`, `division`)
   * Select important features

2. **Exploratory Data Analysis (EDA)**

   * Correlation heatmap
   * AQI distribution by district & season
   * Pollutant contribution analysis

3. **Modeling**

   * **Regression**: Linear Regression, Random Forest, XGBoost
   * **Classification**: Logistic Regression, Random Forest, XGBoost

4. **Evaluation**

   * Regression → RMSE, MAE, R²
   * Classification → Accuracy, F1-score, Confusion Matrix

5. **Deployment**

   * Streamlit dashboard → User enters weather & location → Predicts AQI + Category

🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/air-quality-prediction.git
cd air-quality-prediction

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run app.py

📌 Results (Expected)

* Accurate AQI predictions (R² > 0.85 with XGBoost)
* Pollution category classification with a high F1-score
* Interactive dashboard for district-wise health alerts

🌟 Future Improvements

* Use **LSTM / Prophet** for time series forecasting
* Integrate **real-time API data** (weather + pollutants)
* Mobile app version for wider public use

 👨‍💻 Author
MD.Tanbin Emon
Final  Project – Skills Jobs Course 

