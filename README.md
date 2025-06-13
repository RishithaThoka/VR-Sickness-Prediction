# VR-Sickness-Prediction
This repository implements a machine learning pipeline to predict VR sickness using body movement and demographic data. It employs Logistic Regression, Random Forest, Linear SVM, AdaBoost, and XGBoost to classify users' likelihood of experiencing VR sickness, with model performance evaluated via accuracy, precision, and more.
# Project Overview
The goal of this project is to predict VR sickness using machine learning techniques. The notebook processes data, selects the top features, trains multiple models, and evaluates their performance using metrics like accuracy, precision, recall, F1-score, and ROC-AUC. Visualizations, such as a parallel coordinates plot, are used to explore feature relationships, though a known issue with the plot's color property needs resolution.
# Dataset
The dataset includes features derived from body movement (e.g., anterior-posterior and mediolateral metrics during inspection and search tasks) and demographic information (e.g., age, weight, years of gaming experience). The target variable is binary, indicating whether a subject experienced VR sickness (1) or not (0). The notebook attempts to load data from an Excel file, but some worksheets are missing, as indicated by error messages.
- Note: The dataset is not included in this repository due to potential size or privacy concerns. Users must provide their own dataset in the expected format.
# Features
The top 10 features selected for modeling are:
- Anterior_Posterior_Std_Inspection_Task
- Anterior_Posterior_Mean_Search_Task
- Anterior_Posterior_Mean_Inspection_Task
- Anterior_Posterior_Std_Search_Task
- Mediolateral_Mean_Search_Task
- Years_Played_Games
- Mediolateral_Std_Inspection_Task
- Weight_lbs
- Age
- Mediolateral_Mean_Inspection_Task
# Models
The notebook evaluates the following models:
- Logistic Regression
- Random Forest
- Linear SVM
- AdaBoost
- XGBoost
- Model performance is compared based on accuracy, precision, recall, F1-score, ROC-AUC, and cross-validated F1 scores.
# Results
Model performance metrics are printed in the notebook. Key findings:
- Logistic Regression: Highest accuracy (0.583) but low recall for class 1 (0.3).
- XGBoost: Best cross-validated F1 score (0.6496).
- AdaBoost: Highest recall for class 1 (0.8) but low precision (0.4).
- A comparison table and visualizations (e.g., bar plots) are generated to summarize results.
# License
This project is licensed under the MIT License. See the LICENSE file for details.
