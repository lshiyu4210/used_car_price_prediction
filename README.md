# **Used Car Price Prediction**

This project builds a **Machine Learning pipeline** to predict used car prices based on vehicle features. Using models like **XGBoost, Random Forest, Ridge, and Lasso regression**, the pipeline optimizes predictive performance across **MAE, RMSE, and R²** metrics. The dataset was sourced from **Kaggle** and preprocessed with robust techniques, including multivariate imputation and scaling.

## **Project Overview**
- **Objective**: Predict used car prices using machine learning models.
- **Dataset**: Sourced from [Kaggle](https://www.kaggle.com/datasets/taeefnajib/used-car-price-prediction-dataset), containing **4009 rows** and **10 features**.
- **Methods**:
  - Preprocessing: Categorical encoding (OneHotEncoder), XGB-based imputation, StandardScaler.
  - Model Evaluation: Looping over 5 random states, cross-validation, and GridSearch for hyperparameter tuning.
  - Feature Importance: Global (permutation, gain, weight) and local (SHAP force plots) interpretability.

## **Results**
- **Top Model**: XGBoost Regressor  
- **Best Metrics**:  
    - MAE: 0.0854  
    - RMSE: 0.1107  
    - R²: 0.9041  

## **Python and Package Versions**
The project was developed using the following tools:  

- **Python**: 3.12.5  
- **Key Packages**:  
    - `pandas==2.2.2`  
    - `numpy==1.26.4`  
    - `scikit-learn==1.5.1`  
    - `py-xgboost==2.1.1`  
    - `shap==0.45.1`  
    - `matplotlib==3.9.2`  
    - `plotly==5.23.0`  

For easy setup, install the dependencies via the provided **environment.yaml** file.

---

## **Setup Instructions**

1. Clone this repository:
   ```bash
   git clone https://github.com/lshiyu4210/used_car_price_prediction.git
   cd used_car_price_prediction
   ```

2. Create a virtual environment:
   ```bash
   conda env create -f environment_updated.yaml
   conda activate used_car
   ```

3. Run the pipeline:
   ```bash
   python main.py
   ```

---

## **environment.yaml**

The updated environment file is provided as **environment_updated.yaml**.

---

## **Acknowledgments**
- **Dataset**: [Used Car Price Prediction Dataset](https://www.kaggle.com/datasets/taeefnajib/used-car-price-prediction-dataset)  
- **References**:  
   - Valarmathi et al., 2023  
   - Yılmaz & Selvi, 2023  
