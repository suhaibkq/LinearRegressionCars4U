# 🚗 Cars4U: Used Car Price Prediction

## 📌 Problem Statement

The Indian used car market has outpaced the new car market in recent years. As demand for pre-owned vehicles grows, accurate pricing models are essential. **Cars4U**, a tech start-up, aims to capitalize on this trend by using machine learning to predict the selling price of used cars based on various features.

## 🎯 Objective

To build a regression model that accurately predicts the price of used cars based on factors like age, fuel type, transmission, ownership, mileage, and engine specifications.

## 📊 Dataset

- **File**: `used_cars_data.csv`
- **Target Variable**: `Selling_Price`
- **Key Features**:
  - `Year`, `Present_Price`, `Kms_Driven`, `Fuel_Type`, `Seller_Type`
  - `Transmission`, `Owner`, `Mileage`, `Engine`, `Power`
  - `Seats`, `Car_Name`

## 📁 Repository Structure

├── ML_MLS1_Cars4u.ipynb # Main notebook for data analysis and modeling
├── used_cars_data.csv # Dataset containing historical car data
├── README.md # Project documentation


## 🧪 Project Workflow

1. **Data Preprocessing**
   - Extracted car age from manufacturing year
   - Converted categorical features using one-hot encoding
   - Handled missing and inconsistent values in `Mileage`, `Engine`, and `Power`
   - Dropped irrelevant features like `Car_Name`

2. **Exploratory Data Analysis (EDA)**
   - Analyzed distributions of price, fuel type, and owner history
   - Examined correlations using heatmaps and pair plots

3. **Model Building**
   - Trained multiple models including:
     - Linear Regression
     - Decision Tree Regressor
     - Random Forest Regressor
   - Used GridSearchCV to optimize model hyperparameters

4. **Model Evaluation**
   - Metrics: R² Score, Mean Absolute Error (MAE), Root Mean Squared Error (RMSE)
   - Used cross-validation for generalization performance

## 🏆 Results

- **Best Model**: Random Forest Regressor
- **Performance**: 
  - R² Score: ~0.90+
  - MAE: Significantly lower compared to baseline
- **Top Predictors**: 
  - `Present_Price`, `Car_Age`, `Kms_Driven`, `Fuel_Type_Diesel`

## 🔍 Key Takeaways

- Car age and engine size are strong indicators of price
- Diesel cars tend to retain value better than petrol
- Model performance improves significantly with proper feature engineering

## 🚀 Future Enhancements

- Incorporate car brand/model as a separate encoded feature
- Add geolocation or dealership data for regional pricing
- Deploy as a web app for real-time predictions using Streamlit or Flask

## 👨‍💻 Author

**Suhaib Khalid**  
Machine Learning Enthusiast
