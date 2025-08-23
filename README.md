# HIV Stage Classification and CD4 Improvement Prediction

This project presents an interpretable machine learning pipeline for classifying HIV stages (Early, Mid, AIDS) using structured clinical data. It also includes a secondary binary prediction task to determine whether a patient's CD4 count improves after six months of treatment. The study uses synthetic clinical data derived from the Health Gym initiative and focuses on model transparency, explainability, and clinical relevance.

## Dataset

The dataset contains 8,916 anonymized patient records with the following features:

- Clinical: Baseline CD4 count, viral load, ART drug combination
- Demographic: Gender, Ethnicity
- Derived labels:
  - Multiclass: HIV stage (`Early`, `Mid`, `AIDS`)
  - Binary: CD4 improvement (yes/no after 6 months)

> Source: [Synthetic HIV ART dataset – Health Gym v2.0](https://figshare.com/articles/dataset/22827878)

## Objectives

- Classify patients into clinically defined HIV stages using structured data
- Predict CD4 cell improvement after treatment
- Provide interpretable insights into model predictions using SHAP
- Evaluate fairness across demographic subgroups

## Methodology

- Data preprocessing: label generation, cleaning, encoding
- Model: Random Forest Classifier
- Interpretation: SHAP (TreeExplainer)
- Metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix
- Environment: Jupyter Notebook, Python 3.11

## Key Results

- 100% validation accuracy in stage classification (3-class)
- SHAP plots show CD4 count as the top predictive feature
- Transparent model decisions at both global and individual levels
- Visual analysis by gender and ethnicity for fairness assessment

## Files

- `CD4_Improvement_Prediction_Project.ipynb`: full pipeline with analysis and visualizations
- `Final_CD4_Clinical_Dataset.csv`: structured dataset (synthetic, licensed for academic use)
- `SS25___HIV_Stage_detection_Final-4.pdf`: submitted academic report

## Tools Used

- pandas  
- numpy  
- matplotlib  
- scikit-learn  
- shap  

## Author

Ulukbek Rahmanov  
[LinkedIn](https://www.linkedin.com/in/rulukbek/)
