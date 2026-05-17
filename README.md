# COMPAS Recidivism Bias Analysis

## Project Overview

This project presents a data science analysis of the COMPAS risk assessment system, a tool used in the United States to estimate the probability of criminal recidivism and violent recidivism.

The objective of this analysis is to evaluate the quality of the dataset, study the predictive performance of the COMPAS scores and explore whether the system shows relevant differences in risk assessment across demographic groups such as gender and race.

The project combines exploratory data analysis, feature engineering, confusion matrices, classification metrics and visual analysis to assess both predictive performance and potential fairness issues.

## Objectives

The main objectives of this project are:

- Load and explore the COMPAS dataset.
- Evaluate data quality, including integrity, validity and temporal consistency.
- Analyse whether the variables `is_recid` and `is_violent_recid` are suitable for evaluating COMPAS predictions.
- Create new target variables for general recidivism and violent recidivism within a two-year period.
- Apply a risk threshold of 7 or higher to classify high-risk cases.
- Generate contingency tables and confusion matrices.
- Evaluate false positives and false negatives.
- Compare predictive performance for general recidivism and violent recidivism.
- Explore potential bias in risk scores by gender and race.
- Visualise demographic and predictive patterns in the dataset.

## Dataset

The dataset used in this project is `compas-scores.csv`, which contains information related to defendants assessed by the COMPAS system.

The data includes demographic variables, criminal history, COMPAS risk scores, dates of assessment and information related to subsequent recidivism.

## Methodology

The analysis follows these main steps:

1. Data loading and initial exploration.
2. Data quality assessment.
3. Date conversion and validation.
4. Feature engineering for two-year recidivism.
5. Risk classification using a COMPAS threshold of 7.
6. Confusion matrix analysis.
7. Classification metrics evaluation.
8. Fairness and bias analysis by gender and race.
9. Visual analysis of demographic and predictive patterns.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Repository Structure

```text
compas-recidivism-bias-analysis/
│
├── data/
│   └── compas-scores.csv
│
├── notebooks/
│   └── compas_analysis.ipynb
│
├── requirements.txt
├── README.md
└── LICENSE
```

Key Findings

The analysis shows that COMPAS has moderate predictive capacity for general recidivism, but its performance is more limited when predicting violent recidivism.

The results also highlight an important imbalance between false positives and false negatives. These errors may have different social and judicial consequences.

The analysis suggests that risk scores are not distributed equally across demographic groups. Some groups receive higher average risk scores, which raises questions about fairness, bias and the limitations of algorithmic decision-making in criminal justice contexts.

Ethical Considerations

This project deals with a sensitive topic: the use of algorithmic systems in criminal justice.

The analysis should not be interpreted as a definitive judgement on individual behaviour or criminal risk. Instead, it aims to critically examine the limitations, potential biases and predictive performance of an algorithmic risk assessment system.

The use of this type of tool requires transparency, accountability and careful evaluation of its social impact.

How to Run the Project

Clone the repository:
https://github.com/JOBdeini/compas-recidivism-bias-analysis.git

Install the required dependencies:

pip install -r requirements.txt

Open the Jupyter Notebook:
jupyter notebook


## Author

Developed by Job Delgado Iniesta as part of a Data Science master’s project.

## License

This project is licensed under the MIT License.
