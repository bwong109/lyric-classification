# Song Lyrics Classification
Classifying song lyrics using SVM; includes NLP preprocessing, feature extraction with word embeddings, and SVM optimization via GridSearchCV

## Overview
This repository contains code for classifying song lyrics using Support Vector Machines (SVM). It involves natural language processing to preprocess lyrics, feature extraction using word embeddings, and hyperparameter tuning with GridSearchCV to optimize the SVM model.

## Dataset
The dataset includes song lyrics and their associated labels, stored in "SingleLabel.csv". Pre-trained word embeddings are loaded from "subset.pkl" to convert text data into a numerical format that can be processed by the SVM.

## Preprocessing
Lyrics are preprocessed to remove stopwords and tokenize text, using NLTK's `punkt` and `stopwords` resources. This cleaned text is then transformed into averaged word vectors using the loaded embeddings.

## Model Training and Evaluation
An SVM model is trained with various combinations of parameters (`C`, `gamma`, `kernel`). GridSearchCV is utilized to identify the best parameters based on accuracy. The performance of the best model is presented along with the number of support vectors it uses.

## Results
The script outputs the best hyperparameters, the accuracy of the optimized SVM model, and details about the support vectors, demonstrating the effectiveness of the model in classifying song lyrics.

For more detailed instructions on running the script and a deeper explanation of the methods used, refer to the code documentation within this repository.
