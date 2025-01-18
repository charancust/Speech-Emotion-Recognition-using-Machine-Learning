# Speech-Emotion-Recognition-using-Machine-Learning
This project focuses on developing a Speech Emotion Recognition (SER) system using the techniques of Digital Signal Processing (DSP) and Machine Learning (ML)

Make sure to install the necessary libraries before importing them.

## Data visualization:

The audio files are organized and their paths are stored for further processing.

Emotions are labeled numerically and then mapped to descriptive labels (e.g., 1: neutral, 2: calm, etc.).

The waveplot and spectrogram of different emotions were observed.

## Data augmentation:

Additionally the data was augmented using various Digital Signal Processing techniques.

The following operations were performed:

1. Noise injection

2. Time stretching

3. Pitch shifting

4. Time shifting

## Feature extraction:

The audio pre-processing and feature extraction was done using a library called librosa.

Thsi process involves transforming raw audio signals into meaningful numerical features that can be used by machine learning algorithms.

Relevant features were extracted from the speech segments like,

1. MFCCs (Mel Frequency Cepstral Coefficients):

   Represents the short-term power spectrum of sound.

   Captures vocal tract configuration.

   Based on human auditory perception
   

2. Chroma:
   
   Represent the 12 different pitch classes. So 12-dimensional feature vector.

   Computed from the magnitude spectrogram.

   Captures harmonic and melodic characteristics.

3. Mel spectrogram: Provides a time-frequency representation of the audio.

   Represents frequency content over time.

   Uses mel scale (perceptual scale of pitches).

   Captures energy distribution across frequencies.

   Helps identify emotional patterns in speech.


## Model training:

The data was split into 90% for training and 10% for testing. 

Three models have been implemented,

1. Multi Layer Perceptron (MLP) Classifier:
   
   Hidden layer size: 300 neurons.
   
   Adaptive learning rate.

   Batch size = 256.

2. KNN classifier with k = 5.

3. Random Forest Classifier (RFC) with 100 estimators.

## Performance metrics:

1. Confusion matrix analysis.

2. Classification reports.

3. Accuracy scores for each model.

4. Feature importance visualization (For Random Forest).

## Results:

Comparing the performance metrics of all the models, it can be inferred that the MLP classifier outperformed the other models, indicating its suitability for SER.

## Block diagram:

![image](https://github.com/user-attachments/assets/b3c198f6-f134-45ba-a07f-c652cfd2e5f8)









