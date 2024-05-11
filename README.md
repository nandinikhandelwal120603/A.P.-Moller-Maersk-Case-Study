# A.P.-Moller-Maersk-Case-Study
This assessment appears to involve exploring a dataset related to sourcing products and developing machine learning models to forecast sourcing quantities for June 2021. The tasks involve understanding the data, conducting EDA, handling data quality issues, and implementing forecasting models using Python.


Understanding the Dataset:

1. Each row represents the sourcing of one unit of a product combination.
2. Product combinations are defined by attributes in columns A, B, C, D, E, and F.
3. Multiple rows may have the same combination due to representing 1 unit of sourcing.
4. Training set: July 2020 to May 2021, Test set: June 2021.
5. June 2021 has a single value for each combination, serving as the test set target.

Problem Statement:

Iterate on ML models to predict June 2021 sourcing quantities using training data.
expected Tasks:

1. Understand the dataset and address any open questions.
2. Perform Exploratory Data Analysis (EDA) to gain insights.
3. Utilize Python and its libraries for development.
4. Develop a strategy for handling outliers or poor data quality.
5. Formulate approaches for forecasting June 2021 quantities.
6. Compare and explain different forecasting approaches considered.
7. Explain the final chosen approach and reasoning.


METHODOLOGY:

Dataset Exploration and Preparation:
Explored a dataset containing sourcing cost information.
Performed data cleaning and preparation steps, including handling missing values, checking for duplicates, and conducting univariate analysis.

Model Training and Evaluation:
Trained 6 different models (Linear Regression, Random Forest, FNN, XGBoost, LightGBM, LSTM) to predict sourcing costs.
Saved each model and evaluated its performance on a test dataset using Mean Squared Error (MSE) and Mean Absolute Error (MAE).

Performance Comparison:
Compared the MAE values of various machine learning models on a validation dataset.
Identified Random Forest and XGBoost as the top performers with the lowest MAE values (16.52 and 16.68, respectively), indicating higher accuracy in predicting sourcing costs.

Visualization:
Created a bar plot to visualize and compare the MAE values of different models.
Highlighted performance differences among models, with Random Forest and XGBoost showing the lowest MAE values.

CONCLUSION:
1. In conclusion, our evaluation of various machine learning models using Mean Absolute Error (MAE) as the performance metric revealed that Random Forest, XGBoost, and LightGBM achieved the lowest MAE values. Among these, Random Forest stood out with the lowest MAE of 16.52, indicating its superior accuracy in predicting sourcing costs.
   
3. Random Forest was selected as the optimal model due to its exceptional performance in minimizing the discrepancy between predicted and actual values, as well as its ability to effectively capture underlying data patterns. Moreover, Random Forest demonstrated robustness by providing accurate predictions on unseen data, showcasing its generalizability.
   
5. However, it's imperative to consider additional factors beyond MAE when finalizing the model choice. Factors such as computational complexity, interpretability, and specific requirements of the problem domain should also be taken into account. While Random Forest emerged as the top performer in this analysis, a comprehensive evaluation of all relevant factors is necessary to ensure the most suitable model selection for the task at hand.
