# Sleep-Score-Prediction
This repository implements two approaches for calculating a Sleep Score based on input parameters:

Calculation-Based Approach: A predefined system calculates the sleep score using weighted parameters.

Machine Learning Approach: A predictive system trains models to estimate the sleep score using provided datasets.

Calculation-Based Approach
This approach uses predefined weights to calculate a sleep score based on critical parameters, including:

Fitness Parameters: Steps, Exercise Minutes, and Calories Burned.
Restlessness: Awake Time and Active Sleep.
Sleep Stages: REM, Deep, and Light Sleep.
Other Metrics: Total Sleep Time, Sleep Efficiency, Stress Levels.
Features:
Parameter Weights:
Total Sleep Time: 25%
Sleep Efficiency: 15%
Sleep Stages: 25%
Restlessness: 10%
Fitness: 10%
Stress Recovery: 10%

Grouping similar metrics for efficient scoring.
Dynamic calculation of derived metrics like Sleep Efficiency and Non-REM Sleep.


Machine Learning Approach
This approach trains three machine learning models on a labeled dataset to predict the sleep score:

Random Forest Regressor
Decision Tree Regressor
K-Nearest Neighbors (KNN)

Features:

Data Preparation:

Null values removed for clean training data.
Derived metrics added: Sleep Efficiency and Non-REM Sleep.

Model Training:

Dataset split into training (80%) and testing (20%).
MAE and R² scores used for evaluation.

Input Preprocessing:

Default values for missing input data.
Normalization applied for KNN.
