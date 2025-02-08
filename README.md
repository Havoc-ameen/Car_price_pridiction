# Car_price_pridiction
This repository features a detailed car price prediction project using regression methods. The objective is to enhance prediction accuracy while optimizing models through regularization techniques to prevent overfitting. It's a great resource for those interested in mastering regression models and refining predictive performance.

# 🚗 Car Price Prediction Using Regression Models  

## 📌 Project Overview  
This project focuses on predicting car prices based on key attributes such as brand, manufacturing year, fuel efficiency, and premium features. By leveraging various regression models, the goal is to develop a robust predictive model that accurately estimates the Manufacturer’s Suggested Retail Price (MSRP) while minimizing overfitting.  

### 🔍 Key Techniques Used:  
- Data Cleaning & Processing  
- Exploratory Data Analysis (EDA)  
- Feature Engineering  
- Regularized Regression Models (Lasso, Ridge, Elastic Net)  
- Model Performance Evaluation  

## 📊 Dataset Description  
The dataset consists of **28,143 car records** with 8 key attributes:  

| Feature            | Description |
|--------------------|------------|
| `model_year`      | Manufacturing year of the vehicle |
| `brand`           | Name of the car manufacturer |
| `model`           | Specific car model |
| `type`            | Vehicle classification (SUV, Sedan, Coupe, etc.) |
| `miles_per_gallon` | Fuel efficiency (MPG) |
| `premium_version` | 1 if the car has a premium variant, else 0 |
| `msrp`            | Car price (target variable) |
| `collection_car`  | 1 if the car is considered a collectible, else 0 |

## 🛠 Data Preprocessing  
- **Handling Missing Values:** Imputed or removed as needed.  
- **Outlier Detection & Treatment:** Used **Interquartile Range (IQR) Winsorization** to mitigate extreme values.  
- **Feature Encoding:** Converted categorical variables into numerical format for regression models.  
- **Scaling & Normalization:** Standardized numerical features to improve model stability.  

## 📈 Exploratory Data Analysis (EDA)  
Key insights from data exploration:  
- **Price Distributions:** Luxury brands and premium versions generally have higher MSRPs.  
- **Visualization Techniques:** Used histograms and box plots to analyze trends and detect outliers.  

## 🔮 Regression Models & Performance  

### 1️⃣ Polynomial Regression  
- Applied polynomial transformation to capture nonlinear relationships.  
- **Results:**  
  - **Training Accuracy:** 70.93%  
  - **Testing Accuracy:** -5.76 trillion% (Severe overfitting and model instability)  

### 2️⃣ Regularized Regression Models  
To improve performance and prevent overfitting, we applied **Lasso, Ridge, and Elastic Net Regularization**:  

| Model                  | Training Accuracy | Testing Accuracy |
|------------------------|------------------|------------------|
| **Lasso Regression**   | 63.41%           | 62.68%           |
| **Ridge Regression**   | 63.40%           | 62.68%           |
| **Elastic Net**        | 28.30%           | 28.86%           |

#### 🔍 Observations:  
- **Lasso & Ridge regression** performed similarly, offering a balanced trade-off between bias and variance.  
- **Elastic Net regression** underperformed, indicating that a mix of L1 and L2 penalties was not effective for this dataset.  

## 🚀 Installation & Usage  

### 📌 Prerequisites  
- Ensure you have **Python 3.x** installed along with the required dependencies.  

### 📦 Install Required Libraries  
```bash
pip install pandas numpy matplotlib scikit-learn
```
## 🔧 Running the Project
  ** 1. Clone the repository:**
  ```bash
  git clone https://github.com/Sahil00017/Car-Price-Prediction-Regression
  ```
  ** 2. Navigate to the project folder:**
  ```bash
     cd car-price-regression
  ```
  ** 3. Run the Jupyter Notebook:**
  ```bash
     jupyter notebook "Car_Price_Prediction.ipynb"
  ```
  ** 4. Deactivate the virtual environment when finished:**
  ```bash
     deactivate
  ```
 ## 📌 Key Takeaways
- ✔ Polynomial regression was highly unstable, leading to poor generalization.
- ✔ Lasso and Ridge regression provided the best balance between accuracy and overfitting control.
- ✔ Elastic Net regression performed poorly, showing that a mix of L1 and L2 penalties was ineffective.
- ✔ IQR Winsorization played a crucial role in handling outliers and improving model reliability.

## 📜 License
- This project is licensed under the MIT License.


