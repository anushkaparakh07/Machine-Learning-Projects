# Diabetes Prediction Using Machine Learning

## Project Overview

This project explores diabetes prediction using the **Pima Indians Diabetes Dataset** and a K-Nearest Neighbors (KNN) classification algorithm.

The objective is to analyze patient-related health measurements, explore relationships between features, preprocess the dataset, and build a machine learning model to predict the recorded diabetes outcome.

The project demonstrates an end-to-end introductory machine learning workflow using Python, Pandas, Seaborn, Matplotlib, and Scikit-learn.

## Objectives

- Explore and understand the diabetes dataset using descriptive statistics.
- Identify missing values, duplicate records, and potential outliers.
- Perform exploratory data analysis (EDA) using statistical visualizations.
- Examine correlations between numerical features.
- Standardize input features using `StandardScaler`.
- Train and compare KNN classifiers with different values of K.
- Evaluate classification performance using accuracy, a confusion matrix, precision, recall, and F1-score.

## Dataset Description

The dataset contains patient-related measurements and a binary target variable named `Outcome`.

| Feature | Description |
|---|---|
| `Pregnancies` | Number of pregnancies |
| `Glucose` | Plasma glucose concentration |
| `BloodPressure` | Diastolic blood pressure |
| `SkinThickness` | Triceps skinfold thickness |
| `Insulin` | Two-hour serum insulin |
| `BMI` | Body mass index |
| `DiabetesPedigreeFunction` | Measure associated with diabetes family history |
| `Age` | Age in years |
| `Outcome` | Target class: 0 or 1 |

**Target variable:** `Outcome`

- `0` — Negative class
- `1` — Positive class

The dataset's labels are used for educational classification. Predictions should not be interpreted as medical diagnoses.

## Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Scikit-learn** — Data preprocessing, model training, and evaluation
- **Jupyter Notebook** — Interactive development and analysis

## Project Workflow

### 1. Data Loading and Inspection
- Load the CSV dataset into a Pandas DataFrame.
- Assign descriptive column names.
- Examine dataset structure and descriptive statistics.
- Check for missing values and duplicate records.

### 2. Exploratory Data Analysis
- Visualize the distribution of the target variable.
- Analyze feature distributions using histograms.
- Identify potential outliers using boxplots.
- Explore feature relationships using pairplots.
- Generate a correlation heatmap.

### 3. Data Preprocessing
- Separate input features from the target variable.
- Standardize the numerical features using `StandardScaler`.
- Split the dataset into training and testing subsets.

### 4. Model Training and K Selection
- Implement K-Nearest Neighbors classification.
- Train models using K values from 1 to 14.
- Compare training and testing accuracy.
- Visualize accuracy changes across different K values.

### 5. Model Evaluation
- Evaluate the selected KNN model on the test set.
- Generate a confusion matrix.
- Analyze precision, recall, F1-score, and support using a classification report.

## Installation and Setup

### Prerequisites

- Python 3.9 or later
- Jupyter Notebook or JupyterLab
- pip

### Step 1: Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Diabetes-Prediction.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### Step 2: Navigate to the project directory

```bash
cd Diabetes-Prediction
```

### Step 3: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Diabetes_Prediction.ipynb` and run the cells in order.

Ensure that `pima-indians-diabetes.csv` is available in the same directory as the notebook, or update the dataset path in the code.

## Results and Evaluation

The project compares KNN models across multiple values of K using training and testing accuracy.

The notebook also evaluates the final model using:
- Confusion matrix
- Precision
- Recall
- F1-score
- Classification report

Actual scores should be recorded here after running the notebook and verifying the evaluation results. Model performance may vary depending on preprocessing and the train-test split.

## Limitations

- The project uses a specific dataset and may not generalize to other populations.
- Potentially invalid zero measurements require further investigation.
- Accuracy alone may not adequately represent performance across both classes.
- Further improvements could include cross-validation, hyperparameter tuning, and more systematic handling of data quality.
- This project is for educational purposes and is not intended for clinical use.

## Future Improvements

- Use a Scikit-learn pipeline to prevent data leakage during preprocessing.
- Apply stratified train-test splitting and cross-validation.
- Compare KNN with Logistic Regression, Decision Tree, Random Forest, and other classifiers.
- Tune hyperparameters and evaluate class-specific metrics.
- Add a Streamlit interface for interactive predictions.
- Improve documentation with verified evaluation results and visualizations.

## Author

**Anushka Parakh**

GitHub: (https://github.com/anushkaparakh07/)

---

If you find this project useful, consider giving the repository a star.
