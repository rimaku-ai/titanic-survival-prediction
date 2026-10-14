# Titanic Survival Prediction 🚢

A machine learning project that explores passenger survival on the Titanic dataset and builds Logistic Regression models to predict survival.

## Project Overview

This project follows a structured machine learning workflow, from exploratory data analysis to model interpretation.

The main objectives are to:
- Explore relationships between passenger features and survival.
- Analyze numerical and categorical variables.
- Engineer meaningful features.
- Build and compare Logistic Regression pipelines.
- Evaluate model performance and investigate prediction errors.
- Interpret model coefficients.

## Dataset

The dataset is loaded from Seaborn's built-in Titanic dataset.

The target variable is `survived`:
- `0`: Did not survive
- `1`: Survived

## Exploratory Data Analysis

The analysis examines:
- Age and fare
- Gender and survival rates
- Passenger class
- Family-related features
- Associations between categorical variables using Cramér's V

Key patterns explored include differences in survival rates by gender, passenger class, and family size.

## Feature Engineering

The project creates the following features:

| Feature | Description |
|---|---|
| `family_size` | Total number of family members aboard, including the passenger |
| `family_group` | Groups passengers by family size |
| `sex_class` | Combines gender and passenger class |
| `sex_family` | Combines gender and family group |

## Machine Learning Pipeline

The project uses Logistic Regression with preprocessing pipelines that include:
- Missing-value imputation
- One-hot encoding of categorical variables
- Feature scaling
- Column-wise preprocessing with `ColumnTransformer`

Two model configurations are compared using the same train-test split.

## Model Evaluation

The notebook evaluates the models using classification reports and confusion matrices. It also examines prediction errors and analyzes Logistic Regression coefficients.

No performance score is reported here; consult the notebook for the actual evaluation results.

## Project Structure

```text
titanic-survival-prediction/
├── notebooks/
│   └── titanic_survival_analysis.ipynb
├── README.md
└── requirements.txt
```

## Installation

Clone the repository and move into the project directory:

```bash
git clone <your-repository-url>
cd titanic-survival-prediction
```

Install the dependencies:

```bash
python -m pip install -r requirements.txt
```

## Run the Notebook

Start Jupyter:

```bash
jupyter notebook
```

Open `notebooks/titanic_survival_analysis.ipynb` and run the cells.

## Technologies

- Python
- Pandas
- NumPy
- Seaborn
- SciPy
- Scikit-learn
- Jupyter Notebook

## License

No license has been specified yet.
