#Earthquake Magnitude Prediction using Machine Learning
Overview
This project focuses on predicting earthquake magnitudes using advanced machine learning techniques. Each year, thousands of earthquakes occur worldwide, causing significant human and economic losses. By leveraging regression models and robust data preprocessing, this project aims to develop a system that provides accurate earthquake magnitude predictions, ultimately aiding disaster preparedness and response strategies.

Problem Statement
Accurate prediction of earthquake magnitudes is crucial for mitigating the impacts of natural disasters. This project aims to build a reliable machine learning model to estimate earthquake magnitudes based on seismic features, such as depth, location, and recorded significance, moving beyond traditional statistical methods.

Methodology
1. Exploratory Data Analysis
Objective: Understand the dataset's structure, key variables, and relationships between features.
Key Variables:
Magnitude: Quantitative measure of the seismic energy released.
Depth: Depth of the earthquake's epicenter (in kilometers).
Latitude/Longitude: Geographic coordinates of the epicenter.
Alert: Categorized levels of alert ('green', 'yellow', 'orange', 'red').
Nst: Number of seismic stations that recorded the event.
Significance: A score summarizing the earthquake's overall importance.
2. Data Preprocessing
Handling Missing Values:
Applied predictive imputation for the alert column using Random Forest.
Removed columns with excessive missing values that were non-essential.
Outlier Detection and Treatment:
Used the Interquartile Range (IQR) method to identify and mitigate extreme values.
Ordinal Encoding:
Converted categorical alert levels into numerical values: 'green' → 0, 'yellow' → 1, 'orange' → 2, 'red' → 3.
Feature Selection:
Retained only predictive features, removing irrelevant or redundant columns.
3. Model Development
Training and Testing Split:
Split the dataset into 80% training and 20% testing sets.
Algorithms Used:
Random Forest Regressor: Ensemble learning method combining decision trees.
Gradient Boosting Regressor: Builds sequential models to minimize prediction errors.
Hyperparameter Tuning:
Used GridSearchCV with 5-fold cross-validation to optimize model parameters.
4. Model Evaluation
Compared models using the following metrics:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
R-squared (R²)
5. Model Selection
Gradient Boosting Regressor achieved the best performance:
MAE: 0.0265
MSE: 0.0034
Getting Started
Prerequisites
Python 3.x
Required libraries: Pandas, Scikit-learn, Matplotlib, Seaborn, NumPy
Installation
Clone the repository:
bash
Copier le code
git clone https://github.com/your-repo-link/Earthquake-Magnitude-Prediction.git
cd Earthquake-Magnitude-Prediction
Install dependencies:
bash
Copier le code
pip install -r requirements.txt
Usage
Place the dataset (earthquakes.csv) in the project directory.
Open and run the Jupyter Notebook:
bash
Copier le code
jupyter notebook Earthquake_Project_v2.ipynb
Results
Gradient Boosting achieved the best performance metrics and was selected as the final model.
Visualizations:
Correlation heatmaps and scatter plots illustrate feature relationships.
Performance metrics demonstrate model accuracy and reliability.
Contributors
This project was collaboratively developed by:

El Hilali Nabil
Majdoubi Ilyas
El Magroua Rachid
Darraz Anas
Conclusion
Predicting earthquake magnitudes is a complex yet essential task for disaster management. Using machine learning models like Random Forest and Gradient Boosting, we achieved promising results, highlighting the potential of AI in advancing seismic risk management.

