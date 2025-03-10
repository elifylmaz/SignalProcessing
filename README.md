# Audio Classification and Predictive Maintenance Project

This repository contains the implementation and report of a project focused on audio classification and predictive maintenance tasks. The project worked on two main tasks using machine learning and deep learning techniques.

## Project Overview

The project is divided into two main parts:

1. **Audio Classification**: Various models were used to classify 27 different audio commands.
2. **Predictive Maintenance Classification**: Predicting system health and identifying specific failure types using a standard dataset.

## Audio Classification

- **Dataset**: 3988 audio files with 27 unique labels.
- **Preprocessing**:

- Feature extraction: MFCC (13 features), Mel Spectrogram (128x128).
- Data augmentation: Noise addition, time stretching, pitch shifting.
- **Models Evaluated**:
- **LSTM**: 89.35% test accuracy
- **Traditional ML Models**:
- SVM: 96% accuracy
- Random Forest: 94% accuracy
- Others: Logistic Regression, KNN
- **Main Findings**:
- SVM achieved the highest accuracy among traditional ML models.
- Data imbalance was addressed with boosting techniques.

## Predictive Maintenance Classification

- **Dataset**: Standardized feature dataset containing 9 classes including "Healthy".
- **Preprocessing**:
- Balancing: Oversampling to 48 examples for each class.
- Data augmentation: Adding noise, scaling, reversing feature order.

- Feature extraction: STFT, frequency band features.

- **Models Evaluated**:

- **9 Class Classification**:
- CNN: 88.8% test accuracy
- LSTM: 83.2% test accuracy
- Random Forest: 93.6% test accuracy
- **Binary Classification** ("Healthy" vs "Not Healthy"):
- CNN: 91.2% test accuracy
- LSTM: 89.58% test accuracy
- **8 Class Classification** (specific fault types):
- Random Forest: 92.21% test accuracy
- CNN: 92.21% test accuracy
- LSTM: 83.12% test accuracy
- **Main Findings**:
- Random Forest performed best in multi-class classification.
- CNN achieved high accuracy in both binary and multi-class tasks.

## Conclusion

- In audio classification, SVM provided the best performance among traditional ML models, while LSTM was effective for sequential data.
- In predictive maintenance, Random Forest and CNN models showed superior performance in multi-class and binary classification tasks.
- Future work can focus on further improving model accuracy with data augmentation techniques and feature engineering.
