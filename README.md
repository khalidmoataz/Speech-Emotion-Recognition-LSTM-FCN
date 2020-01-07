# Speech Emotion Recognition LSTM+FCN
Speech Emotion Model determines the emotion from speech with two categories which are happy and sad

## Introduction
Classifying WAV files to emotions happy and sad using Fully convolution neural network and LSTM
Please see the references section at the bottom of this readme for articles on this or related topic.

Steps for classifying audio :
 - Read dataset using libROSA load function to load all files
 - Extract features using libROSA MFCC function to 15 mfcc coefficients
 - Split data into training and testing data
 - Apply training dataset to the model to train
 
## Feature Extraction
We used MFCC to extract features from audio files where each audio file has 16khz sample rate and mono channel each file has 15 mfcc 
coefficients each one of the mfcc has vectors of features

## Main Libraries Used
- libROSA for feature extraction Using MFCC
- Tensorflow For CNN and LSTM network
- scikit-learn for classification and performance evaluation

## Dataset
Egyption dataset used : 2194 Audio file for classification between happy and sad emotion

## Conclusion
After applying the lstm-fcn model to the data the validation accuracy reached to 94% with 0.06 loss
## References
https://github.com/titu1994/LSTM-FCN/
https://librosa.github.io/librosa/index.html
http://practicalcryptography.com/miscellaneous/machine-learning/guide-mel-frequency-cepstral-coefficients-mfccs/
