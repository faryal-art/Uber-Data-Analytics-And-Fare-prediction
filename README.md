
# 🚖 Uber Data Analytics and Fare Prediction

This repository presents a comprehensive analysis of Uber ride booking data, focusing on **exploratory data analysis (EDA)** and the development of machine learning models for **fare prediction**.  

The objective of this project is to identify patterns in ride behavior, understand factors influencing fares, and build predictive models that estimate ride costs.

---

## 1.  📊 Dataset

- **Source**: Kaggle – [Uber Ride Bookings Dataset](https://www.kaggle.com/)
- 
- **Size**: ~150,000 records, 21 attributes
- 
- **Key Columns**:
- 
  - `Date`, `Time`
  - 
  - `Booking Status`
  - 
  - `Vehicle Type`
  - 
  - `Pickup Location`, `Drop Location`
  - 
  - `Ride Distance`
  - 
  - `Booking Value` (fare)
  -   
  - `Customer/Driver Ratings`
  - 
  - `Payment Method`  

> Note: The dataset is not included in this repository due to licensing restrictions. Users are required to download it directly from Kaggle.

---

## 2.  🛠️ Project Workflow

### 1. Data Preprocessing

- Handled missing and inconsistent values in key attributes such as *Booking Value*, *Ride Distance*, and *Ratings*.  
- Converted `Date` and `Time` fields into appropriate datetime formats.  
- Extracted derived features including **day of the week** and **hour of the day**.  

### 2. Exploratory Data Analysis (EDA)

- **Rides and Revenue Trends**: Daily and weekly ride volumes and revenues.
- **Categorical Feature Analysis**
-    * **Booking Status Analysis**: Distribution of completed, cancelled, and incomplete rides.  
-    * **Vehicle Type Usage**: Frequency distribution of different vehicle categories.  
-    * **Payment Preferences**: Usage analysis of cash, UPI, credit/debit cards, and wallets. 
- **Ratings Distribution**: Comparative study of driver and customer ratings.
-  **Fare Relationships** :Fare vs Distance (Scatter Plot)


### 3. Machine Learning – Fare Prediction

- **Target Variable**: `Booking Value` (ride fare).  
- **Selected Features**: `Ride Distance`, `Avg CTAT`, `Avg VTAT`, `Vehicle Type`, and derived time-based features.
  `Pickup Location`,`Drop Location`,`Hour`,`DayOfWeek`,`Month`,`IsWeekend`, `Driver Ratings`, `Customer Rating`
  
- **Implemented Models**:
  - Linear Regression  
  - Polynomial Regression (degree=2)  
  - Random Forest Regressor  

### 4. Model Evaluation

Performance metrics applied:  
- **Mean Squared Error (MSE)**  
- **Root Mean Squared Error (RMSE)**  
- **R² Score**  

Example result (Linear Regression):  

## 3.  📈 Visualizations
Key insights are supported by visualizations, including:    
- 📌 Total Rides and Revenue Over Time
- 📌Booking Status Breakdown
- 📌Vehicle Type Usage
- 📌Payment Method Preferences
- 📌Day-of-Week Ride Distribution
- 📌Fare Prediction (Actual vs Predicted)
---
## 4.  🚀 Future Enhancements
- Incorporate **location-based clustering** to capture regional pricing variations.  
- Include additional **temporal features** such as holidays, weekends, and peak hours.  
- Experiment with **advanced models** (XGBoost, LightGBM, Gradient Boosting).  
- Perform **hyperparameter tuning** for improved accuracy

---
## 5.  ⚙️ Installation and Usage

1.  Clone this repository:
```bash

git clone https://github.com/faryal-art/Uber-Data-Analytics-And-Fare-prediction.git
cd Uber-Data-Analytics-And-Fare-prediction

2. Install dependencies:

pip install -r requirements.txt

3. Run the Jupyter Notebook:

jupyter notebook UberDataAnalytics.ipynb
```


## 📜 License

This project is licensed under the MIT License. See the LICENSE
 file for details.

