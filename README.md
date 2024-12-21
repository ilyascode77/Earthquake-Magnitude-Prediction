# Earthquake Magnitude Prediction using Machine Learning

## 📖 Overview

This project focuses on predicting earthquake magnitudes using machine learning techniques. By leveraging regression models and advanced data preprocessing, we aim to create an efficient system for estimating earthquake magnitudes, contributing to disaster preparedness and response efforts.

## 🛠 Problem Statement

Earthquakes cause significant human and economic losses. Accurately predicting their magnitude can improve early warning systems and better inform response strategies. This project uses machine learning to move beyond traditional statistical methods, providing a robust and reliable prediction model.

## 🔍 Methodology

1.  **Exploratory Data Analysis**
    *   **Objective:** Understand the dataset and relationships between features.
    *   **Key Features:**
        *   `Magnitude`: Measure of the seismic energy released.
        *   `Depth`: Depth of the earthquake’s epicenter.
        *   `Latitude/Longitude`: Geographic coordinates of the epicenter.
        *   `Alert`: Categorized alert levels (`'green'`, `'yellow'`, `'orange'`, `'red'`).
        *   `Significance`: A score summarizing the earthquake's importance.
2.  **Data Preprocessing**
    *   **Handling Missing Values:**
        *   Imputed missing values in the `alert` column using Random Forest.
        *   Removed columns with excessive missing values and low relevance.
    *   **Outlier Detection:**
        *   Applied the Interquartile Range (IQR) method to handle extreme values.
    *   **Encoding:**
        *   Used Ordinal Encoding to convert alert levels (`'green'`, `'yellow'`, etc.) into numerical values.
    *   **Feature Selection:**
        *   Retained predictive features, removing irrelevant ones.
3.  **Model Development**
    *   **Data Split:**
        *   Divided data into 80% training and 20% testing sets.
    *   **Algorithms Used:**
        *   Random Forest Regressor: Ensemble learning method combining decision trees.
        *   Gradient Boosting Regressor: Sequentially minimizes errors for improved performance.
    *   **Hyperparameter Tuning:**
        *   Used `GridSearchCV` for optimizing model parameters with 5-fold cross-validation.
4.  **Model Evaluation**
    *   Evaluated using the following metrics:
        *   Mean Absolute Error (MAE)
        *   Mean Squared Error (MSE)
        *   R-squared (R²)
5.  **Model Selection**
    *   Gradient Boosting Regressor emerged as the best-performing model.

## 🚀 Getting Started

### Prerequisites

*   Python 3.x
*   Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-repo-link/Earthquake-Magnitude-Prediction.git
    cd Earthquake-Magnitude-Prediction
    ```

3.  **Usage**
    *   Place the dataset (`earthquakes.csv`) in the project directory.
    *   Open the Jupyter Notebook:

        ```bash
        jupyter notebook Earthquake_Project_.ipynb
        ```
    *   Run the cells to preprocess the data, train the models, and evaluate performance.

## 📈 Results

*   **Best Model:** Gradient Boosting Regressor
*   **Performance Metrics:**
    *   MAE: `0.0265`
    *   MSE: `0.0034`

    *Visualizations and metrics are included in the notebook for detailed insights.*

## 👥 Contributors

*   MAJDOUBI Ilyas
*   El Hilali Nabil
*   El Magroua Rachid
*   Darraz Anas

## 🏁 Conclusion

Predicting earthquake magnitudes is essential for mitigating disaster impacts. By combining advanced machine learning models and robust data preprocessing, this project demonstrates the potential of AI in improving seismic risk management.
