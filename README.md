# Breast Cancer Classification Project

## BrainyBeam Internship Submission

**Author**: \[Pawan Kumar Barnawal\]\
**Date**: August 24, 2025

## Overview
This project applies feature extraction and machine learning to classify breast cancer (benign vs. malignant) using the Kaggle Breast Cancer Dataset. The goal is to achieve >90% accuracy, and the model achieved 96.49% accuracy using a Random Forest Classifier with feature selection.

## Dataset
- **Source**: [Kaggle Breast Cancer Dataset](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)
- **File**: `data/breast-cancer.csv`
- **Details**: 569 samples, 30 features, binary target (Malignant/Benign)

## Methodology
1. **Preprocessing**:
   - Dropped irrelevant `id` column.
   - Encoded `diagnosis` (M=1, B=0) using `LabelEncoder`.
   - Scaled features with `StandardScaler`.
   - Split data into 80% training and 20% testing sets (stratified).
2. **Feature Extraction**:
   - Selected top 10 features based on Random Forest feature importance.
3. **Model**:
   - Trained a Random Forest Classifier with 100 estimators.
4. **Evaluation**:
   - Achieved 96.49% accuracy on the test set.
   - Generated a confusion matrix for visualization.

## Requirements
- Python 3.9
- Dependencies listed in `environment.yml`
- Install environment: `conda env create -f environment.yml`
- Activate environment: `conda activate breast_cancer_ml`

## Usage
1. Place `data/breast-cancer.csv` in the project directory.
2. Open and run `main.ipynb` in Jupyter Notebook within the activated environment:
   ```bash
   conda activate breast_cancer_ml
   jupyter notebook

## Results
- **Accuracy**: 96.49%
- **Classification Report**: Included in `main.ipynb` output.
- **Visualization**: Confusion matrix saved as `output/confusion_matrix.png`.

## Project Structure

```
feature-extraction-and-machine-learning/
├── main.ipynb              # Main Python script for Classificaton
├── environment.yml     # Conda environment configuration file
├── data/
│    └── breast-cancer.csv       # Dataset for the Classification
├── README.md          # Project documentation
├── report/
│     └── Task_2_Report.docx        # Report of the project
└── output/
     └── confusion_matrix.png       # Image of confusion matrix

```

## Submission Notes
- Include `main.ipynb`, `environment.yml`, `README.md`, `breast-cancer.csv`, `Task_2_Report`, and `confusion_matrix.png` in the zip file.
- Ensure the Conda environment is reproducible.

### Contact
For questions or issues, contact at connectspawan@gmail.com.
