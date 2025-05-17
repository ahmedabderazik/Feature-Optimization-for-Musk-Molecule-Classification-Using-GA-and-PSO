# Feature-Optimization-for-Musk-Molecule-Classification-Using-GA-and-PSO
Binary classification of musk vs non-musk molecules using feature optimization with Genetic Algorithm (GA) and Particle Swarm Optimization (PSO).
# Musk Molecule Classification with GA and PSO

This project focuses on the classification of molecular conformations as either **musk** or **non-musk** using supervised learning and feature optimization techniques.

## Dataset

- **Source**: UCI Machine Learning Repository (Musk Version 2)
- **Instances**: 6598 conformations derived from 102 molecules
- **Features**: 166 geometric, numeric features
- **Target**: Binary class (1 = musk, 0 = non-musk)

Each row represents a 3D conformation of a molecule. Molecules with at least one musk-like conformation are classified as musk.

## Objectives

- Apply classification models on high-dimensional molecular data
- Perform feature selection using:
  - Genetic Algorithm (GA)
  - Particle Swarm Optimization (PSO)
- Evaluate and compare models using multiple performance metrics

## Models Used

- Random Forest  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)

## Performance Metrics

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  

## Project Pipeline

1. **Preprocessing**
   - Normalization using MinMaxScaler
   - Removing non-informative ID features

2. **Model Training (All Features)**
   - Train baseline models on the full dataset

3. **Feature Selection**
   - Apply GA and PSO for dimensionality reduction

4. **Retrain Models on Selected Features**
   - Evaluate performance improvements

5. **Comparison**
   - Analyze metrics before and after feature selection

## Requirements

- Python 3.x
- pandas, numpy, matplotlib, seaborn
- scikit-learn

Install dependencies:
```bash
pip install -r requirements.txt
