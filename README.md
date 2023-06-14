#Image Caption Generator with VGG16 and LSTM

Dataset link: https://www.kaggle.com/datasets/adityajn105/flickr8k

This repository contains code for an image caption generator using the VGG16 convolutional neural network (CNN) for feature extraction and the LSTM (Long Short-Term Memory) network for caption generation. The model takes an input image and generates a descriptive caption that describes the content of the image.

## Dataset

The image caption generator is trained on a dataset of paired images and corresponding captions. The dataset used for training should follow a specific format:

- **Images**: The images should be in a separate directory, properly preprocessed, and resized to a fixed size (e.g., 224x224 pixels) for consistency. The recommended preprocessing steps include normalization, such as subtracting the mean and dividing by the standard deviation.

- **Captions**: The captions should be in a text file or a structured format, with each line corresponding to an image and its associated caption. Preprocessing of captions involves tokenization, lowercasing, and removing punctuation marks. Special tokens like start-of-sequence (SOS) and end-of-sequence (EOS) tokens can be added to mark the beginning and end of captions.

## Implementation

For smooth implementation of this code it requires a GPU so its recommended to run using kaggle itself.

## Evaluation

The model's performance can be evaluated using various evaluation metrics such as BLEU. These metrics can be calculated by comparing the generated captions against the reference captions from the dataset. Implement the evaluation script or use existing libraries to compute the desired metrics.
