# Task-4-Classification-with-Logistic-Regression.
Build a binary classifier using logistic regression.

Step 1: Load Dataset
The dataset is loaded from a CSV file into a pandas DataFrame, which contains tumor data along with their labels (malignant or benign).

Step 2: Data Preprocessing
Irrelevant columns like id and Unnamed: 32 are removed. The diagnosis column is converted from categorical values ('M', 'B') to numeric values (1 for malignant, 0 for benign).

Step 3: Handle Missing Values
Missing values in the dataset are handled using SimpleImputer, which replaces them with the mean value of the respective column to ensure completeness of the data.

Step 4: Prepare Features and Labels
The dataset is divided into features (X) and target labels (y). The features represent measurements of the tumors, and the target label is whether the tumor is malignant or benign.

Step 5: Standardize Features
The features are standardized using StandardScaler, which scales them to have a mean of 0 and a standard deviation of 1. This helps improve the model’s performance.

Step 6: Train/Test Split
The dataset is split into training and testing sets, with 80% of the data used for training and 20% for testing. This allows the model to be evaluated on unseen data.

Step 7: Train Logistic Regression Model
A logistic regression model is trained on the training data. It learns to predict the probability of a tumor being malignant based on the features.

Step 8: Evaluate Model
The model is evaluated on the test data using metrics like accuracy, confusion matrix, precision, recall, and ROC-AUC. These metrics help assess the model’s performance in different areas.

Step 9: Plot ROC Curve
The ROC curve is plotted to visualize the trade-off between the true positive rate and the false positive rate, helping to understand the model's performance across different thresholds.

Step 10: Visualize Decision Boundary (2 Features)
A 2D plot of the decision boundary is created by using just two features, allowing us to visualize how the logistic regression model classifies benign(Blue) and malignant(Red) tumors.

Step 11: Threshold Tuning
The model’s performance is tested at different classification thresholds (0.3, 0.5, and 0.7) to see how it affects accuracy, precision, recall, and ROC-AUC. This helps to adjust the decision-making process based on the problem's needs.
