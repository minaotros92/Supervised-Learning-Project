# Supervised Learning

## Project/Goals
The objective of this project was to used supervised learning techniques to build a machine learning model that can predict whether a patient has diabetes or not, based on certain diagnostic measurements.

## <br>Process
* The project encompassed several initial phases, including exploratory data analysis and data preprocessing. In this process, we worked with the 'diabetes.csv' dataset (which was sourced from Kaggle) to analyze its contents. We created visualizations to investigate relationships between different variables, addressed outliers and incorrect values, standardized the features through data scaling, and conducted necessary feature engineering.

* Once these preliminary tasks were completed, we proceeded to build machine learning models. These models were employed to predict whether a patient has diabetes or not. We evaluated their performance using relevant metrics like accuracy, precision, and recall. Additionally, we ensured that at least one ensemble model was included in our selection of machine learning models for comparison. This comparative analysis aimed to provide valuable insights that could inform decision-making in response to the business questions at hand
The project encompassed several initial phases, including exploratory data analysis and data preprocessing. In this process, we worked with the 'diabetes.csv' dataset (which was sourced from Kaggle) to analyze its contents. We created visualizations to investigate relationships between different variables, addressed outliers and incorrect values, standardized the features through data scaling, and conducted necessary feature engineering.

Once these preliminary tasks were completed, we proceeded to build machine learning models. These models were employed to predict whether a patient has diabetes or not. We evaluated their performance using relevant metrics like accuracy, precision, and recall. Additionally, we ensured that at least one ensemble model was included in our selection of machine learning models for comparison. This comparative analysis aimed to provide valuable insights that could inform decision-making in response to the business questions at hand


## <br>Results
Exploratory Data Analysis (EDA) and Feature Engineering
- During the EDA phase, several important observations and actions were made to enhance the quality of the data:

- Outliers and Data Imbalance: It was noted that outliers, data imbalance, and incorrect values were present. For instance, some predictor variables such as 'Glucose,' 'BloodPressure,' 'SkinThickness,' 'Insulin,' and 'BMI' had zero values, which were not meaningful in this context. To address this issue, two approaches were employed:

- Rows with zero values were either removed from the dataset.
- Zero values were replaced with the median value for those variables.
- Data Scaling: Given the diverse unit representations and magnitudes across different features, data scaling was applied. For example, while 'Pregnancies' ranged from 0 to 17, 'Glucose' ranged from 0 (after removing zero values) to 199. Scaling the features standardizes their ranges, ensuring that each feature contributes fairly and effectively during the model learning process.

- Feature Selection: To streamline the dataset and reduce model complexity, only relevant features were retained. The selection of these features was based on their correlation with the target variable 'Outcome.' This process aimed to enhance the model's performance and interpretability by focusing on the most influential predictor variables.

- By addressing outliers, balancing the data, scaling features, and selecting relevant predictors, the EDA and feature engineering steps played a crucial role in preparing the data for further analysis and modeling

### Training the Machine Learning Model
- We conducted an evaluation of three different machine learning models: logistic regression, support vector machines, and random forest classifiers.

- In our comparison of these models, we considered the following aspects:

- The primary objective was to assess and contrast their performance to understand how they varied in predictive capabilities.

- We used various evaluation metrics, including accuracy, precision, recall, F1-score, and ROC-AUC, to comprehensively evaluate their effectiveness.

- A ROC-AUC plot was generated, providing a visual representation of the performance of all three models.

- Furthermore, we examined the confusion matrices for each of the three models to gain insights into their classification results.

- Overall, it was observed that the support vector machine (SVM) demonstrated the most robust performance in the context of this binary classification task.

- Surprisingly, the random forest classifier ensemble did not outperform the other models, despite conventional expectations that ensemble methods excel in predictive tasks. Several factors may have contributed to this outcome, including the assumptions made during feature selection, the absence of hyperparameter tuning, inadequate handling of data imbalances, and the potential lack of diversity within the ensemble, which can impact its predictive capacity.

## <br>Challenges
- The time constraint posed a significant limitation on the feasibility of specific tasks.
- There was a need to make decisions on how to address issues related to outliers, incorrect data, and data imbalances effectively.
- Choosing the most suitable machine learning models for the analysis was a critical consideration.

## <br>Future Considerations
- We conducted experiments by employing two different approaches: one using top correlated features and another using all available features. This allowed us to assess how each approach influenced model performance.

- We also explored the possibility of enhancing the performance of the random forest ensemble through hyperparameter tuning, aiming to optimize its predictive capabilities.

- In addition to the models we previously analyzed, we considered the implementation of other machine learning algorithms, such as XGBoost, to further diversify our modeling techniques and potentially improve predictive accuracy
