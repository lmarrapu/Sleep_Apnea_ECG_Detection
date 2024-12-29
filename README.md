# 🛌 Unveiling Sleep Dynamics: Apnea Detection with Hidden Markov Models

## 🌟 Overview
This project leverages the Hidden Markov Model (HMM) to classify respiratory events and sleep stages from polysomnographic data, focusing on detecting sleep apnea. Using the MIT-BIH Polysomnographic Database, we developed a system that integrates sequential analysis for healthcare applications.

## ✨ Key Features
- **Sleep and Respiratory Event Classification**: Classifies sleep stages (REM, non-REM) and respiratory events (apnea, hypopnea).
- **HMM-Based Approach**: Utilizes the sequential nature of HMMs to decode sleep stages and detect abnormalities.
- **Class Imbalance Handling**: SMOTE was employed to address underrepresented events and improve model performance.

## 🛠️ Methodology
1. **Data Preprocessing**:
   - Parsing annotations for synchronization with signal data.
   - Noise removal using Butterworth bandpass filtering.
   - Segmentation into overlapping time windows for time-series analysis.

2. **Feature Engineering**:
   - Statistical, morphological, and frequency-domain features (e.g., skewness, kurtosis, entropy).
   - Power spectral density for frequency analysis.

3. **Model Training**:
   - Respiratory event classification using HMM with Gaussian emissions.
   - Sequence decoding for sleep stage prediction.

4. **Evaluation**:
   - Metrics: Accuracy, precision, recall, F1-score.
   - Visualization with confusion matrices and heatmaps.

## 📈 Results
- **Respiratory Event Detection**: Moderate performance with 46.5% accuracy.
- **Sleep Stage Classification**: Limited accuracy (21.1%), highlighting challenges in distinguishing stages.
- **Insights**: Strong potential for respiratory event analysis; further refinement needed for sleep stage prediction.

## 🔧 Tools and Technologies
- Python: HMM Implementation, `NumPy`, `SciPy`
- Dataset: MIT-BIH Polysomnographic Database

## 🌍 Real-World Applications
- **Sleep Apnea Diagnostics**: Early detection and monitoring of respiratory irregularities.
- **Sleep Studies**: Automated classification of sleep stages to support research and treatment.

## 🚀 Future Scope
- Explore advanced models like LSTM or Transformer-based approaches for better temporal sequence learning.
- Enhance feature extraction for improved sleep stage classification.


