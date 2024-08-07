# Musical Chord Classifier
---
![Piano Keys](images/piano_keys.jpg)

## Project Overview
This project aims to classify musical chords using various machine learning models, including a Convolutional Neural Network (CNN). The dataset consists of features extracted from audio files, representing different musical chords.

--- 
## Spectogram Analysis of a Signal
![Spectogram Analysis](images/spectogram_analysis.png)

---
## Dataset
The dataset is imbalanced and consist of two classes, major and minor chords. They stored as audio files 
([Download Dataset](https://www.kaggle.com/datasets/deepcontractor/musical-instrument-chord-classification/data))

---
## Data Preprocessing
- Harmonic features were extracted from audio data using Fourier Transform.
- The dataset was standardized for uniform feature scaling.

### Harmonic Frequencies
![Harmonic Frequencies](images/harmonic_Frequencies.png)

---
## Feature Engineering
- Harmonic intervals between successive harmonics and between harmonics and the first harmonic were calculated.

## Models
- Various models were trained, including Logistic Regression, K-Neighbors Classifier, Decision Tree, Random Forest.
- Hyperparameter tuning was performed to optimize model performance. The Random Forest Classifer was the top performing model; therefore, we only performed a hyperparamter tuning on it.
- Out of curiosity, we also developed a CNN (deep learning model) to see how well it would perform. Its performance was 94.6%

---
## Results
- The Random Forest Classifier perofrmed (95.0%) slightly better the CNN Classifier (94.6%)
- The results analysis was focused on the best classifier (Random Forest)

### Confusion Matrix
![RF Confusion Matrix](images/rf_confusion_matrix.png)

- Precision for Class 1: 96.0%    | Precision for Class 2: 94.4%
- Recall for Class 1: 96.0%       | Recall for Class 2: 94.4%
- F1 Score for Class 1: 96.0%     | F1 Score for Class 2: 94.4%

- Overall, the model performs well with high precision, recall, and F1 scores for both classes. It shows a good balance between precision and recall, indicating that the model is effective at classifying both classes with minimal misclassifications.

---
### ROC
![RF Percision Recall Curves](images/rf_percision_recall_curves.png)

- The Precision-Recall AUC is 0.99, which is very high. This indicates that the model has excellent performance, especially in distinguishing between the two classes.

---
## Setup and Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/khaledalrashid1/musical-chord-classification.git
   cd musical-chord-classification
