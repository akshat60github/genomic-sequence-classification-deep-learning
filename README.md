# Deep Learning–Based Sequence Classification in Genomics
The project explores how different nucleotide encoding strategies and neural network architectures affect performance on a binary DNA sequence classification task.

The work is based on and extended from the official tutorial notebook:
A Primer on Deep Learning in Genomics by Abid et al.

## Problem Statement

The goal of this project is to:

Convert raw DNA sequences into numerical representations

Train and evaluate Artificial Neural Networks (ANNs) and 1D Convolutional Neural Networks (CNNs)

Compare encoding methods, model depth, and activation functions

Ensure reproducibility, fair evaluation, and proper diagnostic reporting

## Dataset & Task

Task: Binary classification of DNA sequences

Input: Nucleotide sequences (A, C, G, T)

Labels: Binary (as provided in the tutorial dataset)

Splits: Train / Validation / Test (70 / 15 / 15) with fixed random seeds

Any dataset slicing or preprocessing steps are clearly documented in the notebook.

## Experiments Performed
### 1️⃣ Nucleotide Encoding Strategies (ANN)

Three encoding techniques were implemented and evaluated using a minimal ANN:

Label Encoding

One-Hot Encoding

FCGR (Frequency Chaos Game Representation)

Each encoding was analyzed with respect to:

Model performance

Convergence behavior

Pros and cons for genomic learning tasks

### 2️⃣ Training Diagnostics & Model Validity

For the best-performing ANN:

Class balance verification

Training & validation loss/metric curves

Overfitting / underfitting analysis

Final test evaluation with:

Accuracy

Precision

Recall

F1-score

ROC-AUC

Confusion Matrix

### 3️⃣ ANN Depth & Activation Study

Controlled experiments were conducted to study:

Effect of increased network depth

Impact of linear activations

Performance comparison with sigmoid activations

All experiments maintain:

Fixed training protocol

Comparable parameter counts

Clear performance interpretation

### 4️⃣ CNN for Sequence Classification

A 1D Convolutional Neural Network was implemented and compared against ANN models:

Explanation of CNN suitability for genomic sequences

Model with multiple convolutional blocks

Performance comparison and architectural justification

## Reproducibility

To ensure reproducibility:

Random seeds fixed (Python, NumPy, TensorFlow)

Single reusable train/validation/test split function

Unified metric reporting utility for all experiments

## 🛠 Tools & Technologies

Programming: Python

Deep Learning: TensorFlow / Keras

Data Processing: NumPy, Pandas

## References

Abid et al., A Primer on Deep Learning in Genomics

COSMIC / TCGA concepts referenced for biological context

## ✨ Author

Akshat Kumar
B.Tech CSE & Biosciences, IIIT Delhi

Visualization: Matplotlib, Seaborn

Models: ANN, 1D CNN

Domain: Genomics, DNA Sequence Analysis
