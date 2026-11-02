https://colab.research.google.com/drive/144m0kIFY9W2qMhlN2nyS_QOvsYJsWc7V#scrollTo=Z-Yz3mbbF23o

# Wine Classification Using PCA, LDA and Logistic Regression   

## Project Overview

This project explores wine classification using the Scikit-learn Wine dataset. The objective is to compare Logistic Regression performance using original features, Principal Component Analysis (PCA), and Linear Discriminant Analysis (LDA).

The project demonstrates how dimensionality reduction techniques can simplify datasets while maintaining classification performance.

## Dataset

- Source: Scikit-learn built-in Wine dataset
- Observations: 178
- Original features: 13 numerical features
- Target classes: 3 wine categories

## Tools and Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Google Colab

## Project Workflow

1. Data loading and exploration
2. Exploratory Data Analysis (EDA)
3. Outlier and correlation analysis
4. Train-test split (80:20)
5. Feature standardisation
6. Baseline Logistic Regression
7. PCA dimensionality reduction
8. LDA dimensionality reduction
9. Model evaluation and comparison
10. Data visualisation

## Model Results

| Model | Components | Accuracy |
|---|---:|---:|
| Logistic Regression | 13 | 97.22% |
| PCA + Logistic Regression | 10 | 97.22% |
| LDA + Logistic Regression | 2 | 97.22% |

PCA retained approximately 96.24% of the dataset variance using 10 components.

All three approaches correctly classified 35 out of 36 test observations.

## Key Findings

- PCA reduced the original 13 dimensions to 10 while retaining approximately 96.24% variance.
- LDA reduced the dataset to just 2 components.
- All three models achieved 97.22% test accuracy.
- LDA demonstrated that substantial dimensionality reduction was possible without reducing test accuracy in this experiment.

## Conclusion

This project helped demonstrate the difference between unsupervised dimensionality reduction using PCA and supervised dimensionality reduction using LDA.

While PCA focuses on preserving variance, LDA focuses on separating known classes. In this experiment, LDA achieved the same classification accuracy using significantly fewer dimensions.

## Limitations

The results are based on a single stratified 80:20 train-test split. Further validation using cross-validation and additional data splits would help assess the consistency of model performance.

## Author

Machine Learning and Data Science Portfolio Project
