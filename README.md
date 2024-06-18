# Musical Chord Classification

## Project Overview
This project aims to classify musical chords using various machine learning models, including a Convolutional Neural Network (CNN). The dataset consists of features extracted from audio files, representing different musical chords.

## Data Preprocessing
- Harmonic features were extracted from audio data using Fourier Transform.
- The dataset was standardized for uniform feature scaling.

## Feature Engineering
- Harmonic intervals between successive harmonics and between harmonics and the first harmonic were calculated.

## Models
- Various models were trained, including Logistic Regression, K-Neighbors Classifier, Decision Tree, Random Forest, and CNN.
- Hyperparameter tuning was performed to optimize model performance.

## Results
- The CNN model achieved the highest validation accuracy of over 94%.
- Detailed performance metrics and confusion matrices were analyzed for each model.

## Setup and Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/khaledalrashid1/musical-chord-classification.git
   cd musical-chord-classification
