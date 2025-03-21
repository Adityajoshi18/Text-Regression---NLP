<!-- # Text Regression - NLP

Regression Task to predict a value from [0,3] to determine the degree of offence in the sentences. 


# Dataset and Precprocessing

Dataset was downloaded from kaggle and was preprocessed using keras tokenizer function. Sentences were converted into sequences of integer values and then padded with 0s in the beginning of each sequence  until each sequence has the same length as the longest sequence.

# Model 

Keras embedding layer was used to embed each word in the input sequence into a vector of 100 dimensions. The output from the embedding layer is a 2d matrix.Following embedding layer is a Conv1d layer with 250 filters of size 3 . Finally there are 2 dense layers with relu activation function , as it is a regrssion problem. The best performing weights are stored in '.h5' file.

The same tokenizer function was used for the preprocessing of test set . The best performing weights are loaded into the model and using the predict function degree of offence is predicted for the test set. -->

# Text Regression - NLP

<!-- Developed a Siamese Deep Network called MaLSTM (Manhattan LSTM) to detect similarity between two sentences. -->

## Overview

This project is a **text regression task** that predicts a value from [0,3] to determine the degree of offence in a given sentence. The model is trained using **deep learning techniques**, leveraging **Keras and TensorFlow** to preprocess text and perform regression-based predictions.

## Dataset and Preprocessing

- The dataset was downloaded from Kaggle.
- Preprocessing was done using Keras Tokenizer, which converts sentences into sequences of integer values.
- Sequences were padded with zeros at the beginning to ensure uniform length across all inputs.
- The same tokenizer function was applied to both the training and test datasets.

## Model Architecture

- **Embedding Layer**: Each word in the input sequence is embedded into a **100-dimensional vector**.
- **1D Convolutional Layer**: A **Conv1D** layer with **250 filters of size 3** follows the embedding layer.
- **Dense Layers**: Two **fully connected dense layers** with **ReLU activation** handle regression.
- The model’s best-performing weights are saved in a .h5 file.

## Prediction Pipeline

1. The test set is preprocessed using the **same tokenizer function**.
2. The **best model weights** are loaded.
3. The model predicts the **degree of offence** for each sentence.

## Files Included

- **nlp_train.csv** – Training dataset
- **nlp_test.csv** – Test dataset
- **sample_submission.csv** – Sample output format
- **Text Regression.ipynb** – Jupyter Notebook containing the full implementation

## Installation & Usage

1. Install dependencies:

```bash
   pip install tensorflow keras numpy pandas scikit-learn
```

2. Run the Jupyter Notebook to train and evaluate the model.






