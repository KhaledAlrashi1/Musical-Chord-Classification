# Project: Musical-Chord-Classification

# Summary
### The project aims to classify chords in audio files (generated by piano and guitar) into major or minor categories. It utilizes methods that analyze frequency-domain (visible spikes in frequency) characteristics of notes. We explore various data processing techniques to highlight features that distinguish between chord types. The extracted feature sets are then processed through several machine learning approaches, ranging from traditional ML approaches to complex deep learning architectures. We see that traditional approaches are still very significant in a problem such as this, especially due to the lack of availability of training data to train deeper models.

# Files
* project.ipynb: a Jupyter Notebook that has the Python code along with analysis for the project.
* Audio_Files: is the dataset. It's a folder that contains two folders (Major and Minor). The Major folder has the major chords (audio files), and The Minor folder has the minor chords (audio files).

# Set-up
### 1) Install all the necessary libraries (see the first cells in the Jupyter Notebook)
### 2) Download the dataset (https://www.kaggle.com/datasets/deepcontractor/musical-instrument-chord-classification/code)
### 3) When training the transformer (at the end of the Jupyter Notebook)
* Download the transformer libraries
* Add path to dataset folder in the load_dataset function
