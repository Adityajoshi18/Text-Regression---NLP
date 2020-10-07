# Text-Regression---NLP

Regression Task to predict a value from [0,3] to determine the degree of offence in the sentences. 


# Dataset and Precprocessing

Dataset was downloaded from kaggle and was preprocessed using keras tokenizer function. Sentences were converted into sequences of integer values and then padded with 0s in the beginning of each sequence  until each sequence has the same length as the longest sequence.

# Model 

Keras embedding layer was used to embed each word in the input sequence into a vector of 100 dimensions. The output from the embedding layer is a 2d matrix.Following embedding layer is a Conv1d layer with 250 filters of size 3 . Finally there are 2 dense layers with relu activation function , as it is a regrssion problem. The best performing weights are stored in '.h5' file.

The same tokenizer function was used for the preprocessing of test set . The best performing weights are loaded into the model and using the predict function degree of offence is predicted for the test set.





