The summary of the task 6 jupiter notebook code is:
1. Importing Libraries

Used pandas, numpy for data handling.

matplotlib for plots and visualizations.

sklearn tools:

train_test_split for splitting data,

StandardScaler for normalization,

KNeighborsClassifier for KNN model,

cross_val_score for cross-validation,

accuracy_score, confusion_matrix, classification_report for evaluation.

2. Data Loading and Exploration

Loaded the Iris dataset from Iris.csv.

Printed head, info, class counts, and descriptive statistics.

Visualized data distributions with histograms and scatter matrix.

3. Splitting Data Before Normalization

Split the dataset into training (80%) and test (20%) sets.

This ensures no data leakage when scaling.

4. Normalization (Standardization)

Applied StandardScaler (fit only on training data).

Transformed both train and test sets.

Checked the training data statistics after scaling → mean ≈ 0, std ≈ 1 (confirming correct normalization).

5. Model Selection (Choosing Best K)

Tested values of K from 1 to 20 using 5-fold cross-validation on the training set.

Printed the average CV accuracy for each K.

Plotted the Elbow Curve (CV accuracy vs. K).

Selected the best K (the one with highest CV accuracy).

6. Final Model Training & Evaluation

Trained the KNN model with the best K on the scaled training set.

Evaluated it on the test set:

Printed test accuracy,

Displayed confusion matrix,

Printed precision, recall, and F1-score (classification report).

7. Visualization of Decision Boundaries

Used only the first two features (Sepal Length & Sepal Width, standardized).

Created a meshgrid over the feature space.

Predicted class labels for each grid point → plotted decision regions.

Overlaid the training points with class labels.

final outputs explaination of code:

The code gives you:

A properly normalized dataset,

The best K chosen automatically via cross-validation,

Accuracy and classification report for the test set,

An Elbow plot to visualize accuracy vs. K,

A decision boundary plot to show how KNN separates classes.
