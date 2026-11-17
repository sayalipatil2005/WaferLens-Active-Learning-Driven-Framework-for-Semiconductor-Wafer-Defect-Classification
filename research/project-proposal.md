# WaferWise AI — Research Proposal

## 1. Research Title

**Active Learning for Semiconductor Wafer Defect Classification Using Deep Learning**

## 2. Introduction

Semiconductor manufacturing involves complex production processes where even small defects can affect the quality and reliability of integrated circuits.

Wafer maps represent the spatial distribution of defects across semiconductor wafers. Identifying these patterns helps engineers understand manufacturing problems and improve production quality.

Traditional supervised machine learning approaches require large amounts of labelled data. However, manually labelling wafer maps can be time-consuming and expensive.

This project explores whether active learning can reduce the amount of labelled data required while maintaining reliable wafer defect classification performance.

## 3. Problem Statement

The project investigates two important challenges:

- Classifying semiconductor wafer defect patterns accurately.
- Reducing dependence on manually labelled training data.

Particular attention will be given to class imbalance and the identification of less common defect patterns.

## 4. Research Objectives

1. Understand and analyse the WM-811K wafer map dataset.
2. Explore wafer map patterns and their class distribution.
3. Develop a baseline machine learning classification model.
4. Investigate deep learning approaches, particularly CNNs.
5. Implement and compare different active learning strategies.
6. Evaluate performance under different labelled-data budgets.
7. Study the impact of active learning on rare defect classification.

## 5. Dataset

**Dataset:** WM-811K Wafer Map Dataset

The dataset will be used to study wafer defect classification.

Initial investigation will cover:

- Wafer map structure and dimensions.
- Label availability and missing labels.
- Defect categories and class imbalance.
- Data preprocessing and visualisation.
- Appropriate training, validation and test splits.

Dataset source: https://www.kaggle.com/datasets/qingyi/wm-811k-wafer-map

## 6. Proposed Methodology

### Phase 1 — Dataset Exploration
- Load and inspect the dataset.
- Understand wafer map representations.
- Analyse class distributions.
- Visualise representative defect patterns.

### Phase 2 — Baseline Model
- Prepare the labelled dataset.
- Implement an initial classification model.
- Establish baseline evaluation metrics.

### Phase 3 — Deep Learning
- Develop a CNN-based classifier.
- Train and evaluate the model.
- Investigate class imbalance handling.

### Phase 4 — Active Learning
Compare the following strategies:

1. Random Sampling
2. Uncertainty Sampling
3. Diversity-Based Sampling
4. Hybrid Active Learning

The strategies will select additional samples for simulated annotation during iterative model training.

### Phase 5 — Experimental Evaluation
Compare the strategies using:

- Accuracy
- Macro-F1 score
- Per-class precision and recall
- Rare-class recall
- Label efficiency
- Performance across annotation budgets

Where feasible, experiments will use lot-aware data splitting to reduce the risk of data leakage.

## 7. Research Questions

**RQ1:** Can active learning reduce the amount of labelled data required for wafer defect classification?

**RQ2:** Which active learning strategy provides the best classification performance under a limited annotation budget?

**RQ3:** How do active learning strategies affect the recognition of rare wafer defect patterns?

**RQ4:** Does combining uncertainty and diversity improve classification performance compared with individual strategies?

## 8. Expected Outcomes

The expected outcomes include:

- An exploratory analysis of WM-811K.
- A baseline wafer defect classification model.
- A CNN-based classification approach.
- An experimental comparison of active learning strategies.
- An evaluation of annotation efficiency and rare-class recognition.
- Research documentation and reproducible experiments.

These are planned outcomes, not completed results.

## 9. Technology Stack

- Python
- NumPy and Pandas
- Matplotlib
- Scikit-learn
- PyTorch or TensorFlow
- Jupyter Notebook
- Git and GitHub

## 10. Project Status

**Status:** Research planning and preparation.

Implementation, experiments and evaluation will be documented as the project progresses.

## 11. Research Scope

This is an independent undergraduate research project focused on applying artificial intelligence and active learning to semiconductor wafer defect classification.

The project aims to develop practical knowledge at the intersection of AI, deep learning, computer vision and semiconductor manufacturing.
