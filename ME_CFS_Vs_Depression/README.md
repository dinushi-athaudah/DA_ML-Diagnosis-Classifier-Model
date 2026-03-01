# ME/CFS vs. Depression ML Classification

This project employs a comprehensive machine learning pipeline to systematically differentiate between ME/CFS, Depression, and control cases. By analyzing quantifiable patient characteristics, the study demonstrates the feasibility of automated diagnostic support tools to reduce misdiagnosis rates and improve patient outcomes. 

## Project Structure
- `ME_CFS Vs Depression_ML Classification.ipynb`: Main Jupyter Notebook.
- `Data/`: Folder containing the `me_cfs_vs_depression_dataset.csv`.
- `requirements.txt`: List of Python dependencies.

## Setup Instructions
1. Clone the repository.
2. Install requirements:
   ```bash
   pip install -r requirements.txt
3. Run the notebook using Jupyter:
   ```bash
   jupyter notebook

## Dataset Details

Source: https://www.kaggle.com/datasets/storytellerman/mecfs-vs-depression-classification-dataset

The study utilizes a multi-dimensional dataset of 1,000 patient records with 16 distinct features spanning: 

Clinical Measures: PHQ-9 depression scores, fatigue severity, brain fog, physical pain, and stress levels. 

Sleep & Energy: Sleep quality indices, hours of sleep, and Post-Exertional Malaise (PEM) duration/presence. 

Lifestyle Factors: Work status, social activity, exercise frequency, and mindfulness practices. 

Demographics: Age and gender. 

## Machine Learning Pipeline

The methodology prioritizes data integrity and model robustness through: 

Preprocessing: Statistical distribution-based missing value imputation (Mean/Median/Mode) and outlier removal using the Interquartile Range (IQR) method. 

Addressing Imbalance: Applied SMOTE (Synthetic Minority Oversampling Technique) to ensure balanced representation across diagnostic classes. 

Feature Engineering: Strategic encoding (Binary, Ordinal, and One-Hot) and feature scaling using StandardScaler. 

Model Optimization: Hyperparameter tuning via Grid Search Cross-Validation for multiple algorithms. 

Ensemble Learning: Implementation of a Soft-Voting Ensemble model to leverage the complementary strengths of individual classifiers. 

## Key Results

The project evaluated five core algorithms, with tree-based and linear models showing exceptional performance: 

Decision Tree, Random Forest, & SVM: Achieved a remarkable 99.03% Accuracy and 99.03% F1-score. 

Naive Bayes: Achieved 90.34% Accuracy. 

K-Nearest Neighbors (KNN): Achieved 85.51% Accuracy.

## Contributors
This project was developed as a group assignment for the **DSA 504 2.0 - Machine Learning I** module at the **University of Sri Jayewardenepura**.

* **A.H.G.D.N Athaudahetti**
* **D.A.D.N. Danthapuraarachchi**
* **W.B.A.N. Bandara**
