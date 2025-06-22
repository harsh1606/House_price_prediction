# 🏡 House Price Prediction using Regression Models

## 📌 Overview
This project uses a dataset of over 21,000 properties in King County, USA to build predictive models that estimate house prices based on features like size, number of rooms, location, and construction year. Three approaches were explored:
- **Decision Tree Regression**
- **Linear Regression**
- **OLS Regression (via statsmodels)**

---

## 📁 Dataset Description
- File: `kc_house_data.csv`
- Total samples: 21,613
- Key features include:
  - Bedrooms, Bathrooms, Floors
  - Sqft living/lot, Year built/renovated
  - Zipcode, Latitude, Longitude
  - Waterfront/View indicators

Target variable: `price`  
Excluded variable: `date`

---

## 🔄 Preprocessing Steps
- Dropped non-informative columns: `price`, `date` from features
- Visualized correlation between each feature and target using scatter plots
- Split data into training and test sets (67% / 33%)

---

## 🧠 Models Used

### 1. ✅ Decision Tree Regressor
- Achieved **R² Score**: 0.723  
- Mean Squared Error: ~38.2 Billion  
- Fast, interpretable, and able to capture nonlinear patterns

### 2. 🔢 Linear Regression
- Achieved **R² Score**: 0.702  
- Mean Squared Error: ~41.2 Billion  
- Simple baseline model to benchmark against more complex models

### 3. 📊 OLS Regression (statsmodels)
- Achieved **R² Score**: 0.700  
- Detailed statistical summary including coefficients, p-values, and confidence intervals
- Insights into multicollinearity and variable significance

---

## 📊 Model Comparison
| Model                 | R² Score | Mean Squared Error |
|----------------------|----------|--------------------|
| Decision Tree        | 0.723    | 38.2B              |
| Linear Regression    | 0.702    | 41.2B              |
| OLS Regression       | 0.700    | —                  |

---

## ▶️ How to Run
1. Place `kc_house_data.csv` in your working directory.
2. Install dependencies:
```bash
pip install pandas numpy matplotlib scikit-learn statsmodels
```
3. Run the Python script in your preferred IDE or notebook.

---

## 📌 Final Insights
- Key predictors of house price: `sqft_living`, `grade`, `lat`, `bathrooms`, and `view`
- Waterfront properties and location significantly influence pricing
- OLS revealed multicollinearity in some features

---

## 👤 Author
**Harsh Kumar Tyagi**  
📧 [harshtyagi022@gmail.com](mailto:harshtyagi022@gmail.com)  
🪪 License: MIT
