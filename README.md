# Heart-sound-Classification-Using-RNN

## Introduction

A GRU model for classifying Heart sound signal into 1 of 13 classes.

## Dataset
The dataset used is from the PhysioNet Challenge2016:Heart sound classification in kaggle ([Link](https://www.kaggle.com/datasets/bjoernjostein/physionet-challenge-2016))

## Preprocessing
The data was preprocessed using MATLAB R2023a.
- All the PCG records were cropped at the shortest one (5 seconds), to ensure the consistency of the data intering the model.
- The data were kept at 2k Hz.

## Model selection
Few trials were made with different scienarios, the best was selected.
- Trial 1: The spectrogram were compouted using multitapers, then a CNN were trained to detect the patterns. (77%)

- Trial 2: An LSTM was trained on audio signal. (75%)

## Results
The model reached an accuracy of about 79.85%
