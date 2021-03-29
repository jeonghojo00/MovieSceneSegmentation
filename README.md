# MovieSceneSegmentation
Verify Movie Scene Segmentations by Predictive Optimization

## Data
 - Number of movies: 64
 - Each movie consists of 4 features: ‘place’, ‘cast’, ‘action’, and ‘audio’.

## Method
 - Assuemd binary classification: whehter scene transition or not.
 - Convolutional Neural Network (1D)
 - Bi-LSTM Neural Network

## Process
 - Preprocess the input data into one big dataset with padding at the end of data to make them have the same number of length to train with Neural Network
 - Run CNN1D with 4 features individually
 - Concantenate the 4 features
 - Run RNN with bi-LSTM layers
 
## Train and Testing
 - Trained 80% of moveis with 20%(except 2 movies at the end) of validating
 - Testing with the last two movies. 

## Current result
 - The results are between 0 and 0.4 although I trained with 0 and 1 values as 

## Further development needed
 - Find why results are between 0 and 0.4 and improve the accuarcy
 - Improve execution time.
