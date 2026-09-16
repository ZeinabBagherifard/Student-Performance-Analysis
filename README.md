# Student-Performance-Analysis

This project presents an exploratory data analysis (EDA) and a supervised classification model on the Student Performance dataset from the UCI Machine Learning Repository.

The notebook includes:
- Data cleaning and preprocessing
- Feature selection
- Data type correction
- Exploratory data analysis
- Basic statistical insights and correlations
- A pass/fail classification model built with `scikit-learn` (Logistic Regression and Random Forest)

This notebook was originally developed as part of a university course assignment and later refined for portfolio purposes.

## Classification task

The notebook predicts whether a student **passes** (`G3 >= 10`) or **fails** (`G3 < 10`) the course, based only on
demographic, family, and behavioral features (parental education/job, reason for choosing the school, travel time, study
time, past failures, health, and absences). The first and second period grades (`G1`, `G2`) are deliberately excluded from
the feature set, since they are strongly correlated with the final grade and would otherwise leak the answer into the
model. Two models are trained and compared:

- **Logistic Regression** — a simple, interpretable linear baseline
- **Random Forest** — a non-linear ensemble model, also used to inspect feature importance

Both are evaluated with accuracy, a classification report (precision/recall/F1), and confusion matrices.

## Dataset
Student Performance Dataset  
UCI Machine Learning Repository:  
https://archive.ics.uci.edu/dataset/320/student+performance

## Running the notebook

```bash
pip install pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook student-performance-eda.ipynb
```
