The script trains and evaluates a Support Vector Regression (SVR) model for letter recognition. It loads the dataset, encodes labels numerically, and iteratively (10 times) splits the data into training and testing sets. A pipeline standardizes features and applies SVR. Hyperparameter tuning (kernel, C, epsilon) is performed using GridSearchCV with 3-fold cross-validation in each iteration. The best model's accuracy is evaluated on the test set. A "convergence simulation" tracks accuracy with increasing training data size. Results (accuracy, best hyperparameters) are stored.

Result Table (svm_results.csv)
This table summarizes the 10 evaluation runs, showing:

Sample: Run identifier.
Accuracy: Percentage of correctly classified letters.
Kernel: Best kernel function ('linear', 'rbf', 'poly').
C: Best regularization parameter.
Epsilon: Best epsilon value.
It helps assess performance consistency and identify effective hyperparameters.

Result Graph (Conceptual)
Potential graphs include:

Accuracy Distribution: Shows the spread and central tendency of accuracy across runs.
Convergence Curves: Illustrates accuracy improvement with more training data.
Best Hyperparameter Frequency: Highlights the most frequently selected optimal hyperparameter values.
Comparison of Runs: Directly compares accuracy across the 10 iterations.
These visualizations provide insights into model stability, learning behavior, and impactful hyperparameter choices.
