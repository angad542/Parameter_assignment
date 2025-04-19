This project uses Support Vector Regression (SVR) to predict letter recognition from a dataset of image-derived features.

**Key Features:**

* Loads and preprocesses the letter recognition dataset.
* Performs hyperparameter tuning for SVR using GridSearchCV.
* Evaluates model accuracy across 10 different train-test splits.
* Saves the results (accuracy, best hyperparameters) to `svm_results.csv`.
* Simulates model convergence (accuracy over increasing training data).

**Usage:**

1.  Ensure `letter-recognition.csv` is in the same directory.
2.  Install required libraries: `pip install pandas numpy scikit-learn matplotlib`
3.  Run the script: `python main.py`

The `svm_results.csv` file will contain a summary of the model performance.
