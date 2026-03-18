# AI_Projects
# GDP Prediction Using Machine Learning Techniques

## Project Documentation

**Submitted by:** Ayesha Noor  
**Degree Program:** BS Computer Science  
**Course:** Artificial Intelligence  
**Instructor:** Dr. Naveed Anwar Butt  
**Submission Date:** March 2023  

---

## Abstract
This project aims to predict GDP per capita using different machine learning regression models. The goal was to understand how various socio-economic factors influence GDP and to compare the performance of different algorithms. Models applied include Linear Regression, Support Vector Machine (SVM), Random Forest, and Gradient Boosting. Among these, Random Forest produced the most accurate results, demonstrating that ensemble methods are well-suited for this type of data.

---

## Introduction
GDP per capita is an important metric to evaluate a country’s economic condition, reflecting average income and overall standard of living. Predicting GDP helps in understanding economic patterns and supports planning and analysis.

**Objectives of the project:**
- Explore the relationship between country features and GDP  
- Apply multiple machine learning models  
- Compare model performance  
- Identify the most effective model  

---

## Dataset Description
The dataset used is **`countries_of_the_world`**, containing economic and demographic indicators for various countries.  

**Key features include:**
- Population  
- Area  
- Literacy rate  
- Net migration  
- Industry, agriculture, and service sectors  
- GDP per capita  

---

## Methodology

### Data Loading
The dataset was loaded using the **Pandas** library in Python for processing and analysis.

### Data Preprocessing
- Removed extra spaces from column names  
- Converted numerical values stored as text into numeric format  

### Handling Missing Values
- Identified missing values using `isnull().sum()`  
- Filled missing entries using mean or median values as appropriate  

### Exploratory Data Analysis (EDA)
- `describe()` used for statistical overview  
- Histograms plotted to observe distributions  
- Correlation analysis to identify relationships  
- Pairplots for visual comparison of features  

### Feature Scaling
- Applied where necessary, especially for models sensitive to scale (e.g., SVM)  

### Data Splitting
- Divided dataset into training and testing sets  
- Two approaches: with scaling and without scaling  

### Models Applied
1. Linear Regression  
2. Support Vector Machine (SVM)  
3. Random Forest Regressor  
4. Gradient Boosting Regressor  

### Model Evaluation Metrics
- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

---

## Results and Discussion
| Model | MAE | RMSE | R² Score |
|-------|-----|------|----------|
| Random Forest | 2142.13 | 3097.19 | 0.8839 |
| Gradient Boosting | Slightly lower than Random Forest | - | - |
| Linear Regression | Poor | - | - |
| SVM | Weakest | - | - |

**Insights:**  
- Random Forest performed the best, suggesting ensemble methods handle complex GDP relationships effectively.  
- Gradient Boosting performed well but slightly lower than Random Forest.  
- Linear Regression struggled with non-linear data.  
- SVM showed the weakest performance.  

---

## Conclusion
Different machine learning models were applied to predict GDP per capita. Random Forest achieved the most accurate results, highlighting the importance of choosing the right model for real-world data.

---

## Limitations
- Limited dataset size  
- No historical/time-based data  
- Minimal feature engineering  

---

## Future Work
- Use larger and updated datasets  
- Apply hyperparameter tuning  
- Explore advanced models like XGBoost  
- Perform deeper feature analysis  

---

## Project Structure
