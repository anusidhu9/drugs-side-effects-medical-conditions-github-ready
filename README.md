# Drugs, Side Effects, and Medical Conditions Analysis

A Python data-analysis and machine-learning project that explores relationships among drugs, medical conditions, side effects, drug classes, ratings, reviews, regulatory attributes, pregnancy categories, and alcohol interactions.

## Overview

The project uses exploratory data analysis, preprocessing, visualization, association-rule mining, classification, regression, and clustering techniques.

### Main techniques

- Data cleaning and missing-value handling
- Duplicate detection
- Categorical encoding
- Feature standardization
- Correlation analysis
- Frequency analysis
- Association Rule Mining (Apriori)
- Decision Tree classification
- Support Vector Machine (SVM)
- DBSCAN clustering
- K-Means clustering
- Linear Regression

## Repository Structure

```text
drugs-side-effects-medical-conditions/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── drugs_side_effects_drugs_com.csv
│   └── drugs_side_effects_drugs_com_version2.csv
│
├── notebooks/
│   └── drugs-side-effects-medical-conditions.ipynb
│
└── outputs/
    ├── medical_condition_counts.csv
    ├── side_effect_counts.csv
    └── figures/
```

## Technologies

- Python 3
- pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- scikit-learn
- mlxtend
- Jupyter Notebook

## Setup

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd drugs-side-effects-medical-conditions
```

### 2. Create a virtual environment

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add the dataset

Place the original CSV dataset at:

```text
data/drugs_side_effects_drugs_com.csv
```

The cleaned notebook uses a repository-relative path rather than a personal Windows path.

### 5. Open the notebook

In VS Code, install the **Python** and **Jupyter** extensions, then open:

```text
notebooks/drugs-side-effects-medical-conditions.ipynb
```

Select the project's `.venv` Python interpreter and run the notebook from top to bottom.

## Analysis Workflow

1. Load and inspect the dataset.
2. Check columns, shape, data types, duplicates, and missing values.
3. Convert rating, review, and activity fields to numeric formats.
4. Transform alcohol-interaction information.
5. Fill missing categorical/numeric information according to the notebook's existing rules.
6. Save and reload a cleaned dataset.
7. Encode categorical variables.
8. Standardize selected features.
9. Analyze correlations.
10. Count medical conditions, side effects, and drug classes.
11. Create indicator features for selected side effects, drug classes, and medical conditions.
12. Mine association rules using Apriori.
13. Train and evaluate a decision-tree classifier.
14. Train an SVM classifier.
15. Apply DBSCAN clustering.
16. Explore K-Means clustering.
17. Run the regression analysis included in the notebook.

## Important Reproducibility Note

The original notebook contained computer-specific Windows paths. Those paths have been replaced with repository-relative paths such as:

```python
pd.read_csv("../data/drugs_side_effects_drugs_com.csv")
```

This allows teammates to clone the repository and run the notebook without changing paths.

## Medical/Data Disclaimer

This repository is for educational data-analysis and machine-learning purposes. Statistical relationships, classifications, clusters, or association rules produced by the notebook should not be interpreted as clinical recommendations, diagnosis, treatment advice, or proof of drug safety or effectiveness.

## Dataset

The repository expects the drug dataset used by the original notebook. If redistribution of the dataset is restricted, do not commit the raw CSV; instead, document where authorized users can obtain it.

## Author

Add your name and team members here.

## License

Add the license required by your course, team, or dataset terms.
