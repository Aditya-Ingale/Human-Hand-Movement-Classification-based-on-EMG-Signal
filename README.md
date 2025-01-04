# EMG-Based Hand Movement Classification

## Introduction

This project focuses on the classification of human hand movements using Electromyography (EMG) signals. It explores various feature extraction techniques and machine learning classifiers to achieve accurate hand gesture recognition. The application areas include prosthetics, rehabilitation, and human-computer interaction.

The dataset utilized for this project was sourced from the UCI Machine Learning Repository and includes EMG signals for three classes:

- Hand at Rest
- Wrist Flexion
- Wrist Extension

### Key project achievements:

- Preprocessing using Bandpass and Notch filters.
- Feature extraction using Frequency Domain (FD), Discrete Wavelet Transform (DWT), and Time-Domain & DWT fusion.
- Evaluation with machine learning classifiers: Random Forest (RF), K-Nearest Neighbors (KNN), and Decision Tree (DT).

## Project Flow

### 1. Dataset Collection

- EMG signals collected using MYO Thalmic bracelet with 8 sensors.
- Dataset consists of 15,000 rows per class for 3 gestures.

### 2. Preprocessing

- Filters applied to clean and normalize the signal.
- Signals segmented using a sliding window approach.

### 3. Feature Extraction

- Extracted features include frequency-based metrics, wavelet coefficients, and fused time-domain features.

### 4. Classification

- Classifiers were trained and tested with a 70:30 split for training and testing data.
- Classifiers evaluated based on accuracy, precision, recall, and F1-score.

## Results

### Classifier Performance

| Feature Extractor    | Classifier        | Accuracy (%) |
| -------------------- | ----------------- | ------------ |
| DWT                  | Random Forest     | 80.77        |
| FD                   | Random Forest     | 81.69        |
| Fusion (TD + DWT)    | Decision Tree     | 81.21        |

## Conclusion

This project successfully demonstrates the potential of EMG-based hand gesture classification. The integration of advanced feature extraction techniques and machine learning algorithms provides promising results, paving the way for future applications in assistive technologies and rehabilitation systems.

## References

- International Journal of Electrical and Electronics Research (IJEER)
- Dataset sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/EMG+Hand+Movement+Dataset)
