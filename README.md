# Facial Recognition Methods Evaluation Project

This repository contains a comparative study of different feature extraction techniques and machine learning classification algorithms applied to facial recognition. This project was developed as a final assignment for the **Information Security** course.

**Authors:** Gabriel Beloso and Rafaela Vilela

## 📋 Project Overview

The main objective of this study is to evaluate the performance of various combinations of feature extractors and ML models for facial verification tasks. The evaluation uses 10-fold cross-validation and focuses on metrics crucial for security systems, such as reliability and error rates.

### Techniques used in the study

* **Feature Extraction:**
    * **LBPH** (Local Binary Patterns Histograms)
    * **HOG** (Histogram of Oriented Gradients)
    * **HU Moments** (Invariant Moments)
* **Classification Models:**
    * **SVM** (Support Vector Machine)
    * **KNN** (K-Nearest Neighbors)
    * **RF** (Random Forest)

---

## 📁 Project Structure

The primary notebook handles the entire data pipeline:
1.  Loading the face-pair dataset.
2.  Preprocessing and feature extraction.
3.  Training using 10-fold cross-validation.
4.  Exporting analytical results to disk.

### Generated Outputs (`/results`):
* `metricas_finais.csv`: Consolidated table with accuracy, precision, recall, and F1-score for all combinations.
* `CM_<FEATURE>_<MODEL>.csv`: Detailed Confusion Matrices for error analysis.
* `ROC_<FEATURE>_<MODEL>.png`: ROC Curves to evaluate False Positive vs. True Positive rates.
* `/plots/*.png`: Comparative performance charts.

---

## 🚀 Getting Started

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/gbeloso/facial-recognition-methods-evaluation.git
    ```

2.  **Install dependencies:**
    This project requires Python and standard data science libraries:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Notebook:**
    Open `facial_recognition_methods_eval.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.

---

## 📊 Methodology & Metrics

In the context of Information Security, we evaluate the models based on:
* **Confusion Matrix:** Crucial for identifying **False Acceptance Rate (FAR)** and **False Rejection Rate (FRR)**.
* **ROC Curve & AUC:** To measure the model's ability to distinguish between identities.

* **Cross-Validation:** Ensuring the results are statistically significant and free from overfitting.


