# Heart Disease Prediction 

This project uses the UCI heart disease dataset, which includes health metrics for 303 individuals and a target label indicating whether each patient has heart disease. The dataset includes 13 features, such as age, sex, and cholesterol level, all of which are commonly available in medical records. This study aims to identify patterns in these attributes to predict heart disease, which could lead to earlier and more cost-effective intervention, potentially saving lives.

Data Summary
Dataset Source: UCI Heart Disease Repository
Data Points: 303 records, balanced
Features: 13 health-related attributes, e.g., age, sex, cholesterol level
Experimentation
The dataset was divided into training (80%) and test (20%) sets. I explored multiple machine learning algorithms to develope the best baseline model. 

Decision Tree

Parameters: max_depth and min_samples_split controlled model complexity and helped mitigate overfitting. With a shallow depth, the model generalized better.
Results: Performed well, though overfitting occurred with deeper trees.
k-Nearest Neighbors (KNN)

Parameters: k (number of neighbors) and weighting method (uniform vs. distance).
Results: Optimal performance with k=5. Larger k values reduced the model’s ability to fit the data accurately.
Neural Network (Multi-layer Perceptron)

Parameters: Hidden layer size and maximum iterations.
Results: Showed continuous accuracy improvement with more data but took the longest to train.
Support Vector Machine (SVM)

Parameters: Kernel function and C value.
Results: The polynomial kernel performed best. Higher C values improved training accuracy but introduced overfitting.
Boosted Decision Tree (Adaptive Boosting)

Parameters: Number of weak learners and tree depth.
Results: Performed similarly to Decision Trees, with better generalization on the test set as sample size increased.