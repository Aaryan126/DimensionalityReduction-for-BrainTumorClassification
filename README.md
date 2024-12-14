# Dimensionality Reduction for Classification on Brain Tumor Dataset

## Overview
This project explores the use of dimensionality reduction techniques to enhance the classification accuracy of brain tumor detection using image data. The primary goal is to develop a reliable automated system that can classify brain tumors accurately, which is critical for early diagnosis and treatment planning.

The study applies three dimensionality reduction methods: Principal Component Analysis (PCA), Linear Discriminant Analysis (LDA), and Autoencoders. The reduced-dimensional data is then evaluated using six different classification models.

---

## Project Structure
The repository contains the following key sections:

- **Introduction**: Overview of the problem, significance of brain tumor classification, and project objectives.
- **Pre-processing**: Description of image pre-processing steps including resizing, augmentation, grayscaling, and normalization.
- **Dimensionality Reduction Methods**: Detailed exploration of PCA, LDA, their combination (PCA+LDA), and Autoencoders.
- **Performance Metrics**: Metrics such as accuracy, precision, and recall are used to evaluate the effectiveness of the methods.
- **Classification Models**: Six classifiers (Logistic Regression, Linear SVC, Ridge Classifier, Passive Aggressive Classifier, SGD Classifier, k-Nearest Neighbors) are used for benchmarking the dimensionality reduction methods.
- **Results and Analysis**: Comparison of classifiers' performance with and without dimensionality reduction, along with findings and implications.
- **Code**: Implementation of the methods used in the study (included in Appendix 2 of the report).

---

## Getting Started

### Prerequisites
- Python
- Libraries: `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `tensorflow` (for Autoencoders)

### Dataset
The brain tumor dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/preetviradiya/brian-tumor-dataset). It contains labeled images of healthy and brain tumor cases.

**View results**:
   - Classification accuracy comparisons and all details about the project results can be seen in Report.pdf.

---

## Key Findings

- **PCA** outperformed other methods in terms of preserving classification accuracy while reducing dimensions significantly.
- **PCA+LDA** showed robustness by leveraging variance preservation from PCA followed by class separation by LDA.
- **Autoencoders** excelled with non-linear models like k-Nearest Neighbors (kNN).

---

## Future Work
- Expand to include other brain diseases for diagnosis.
- Improve dimensionality reduction techniques for higher accuracy in real-world applications.
- Optimize computational efficiency for large-scale datasets.
