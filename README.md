# Overcoming short text and multi-class imbalance issues in invoice text classification: A data augmentation and deep learning strategy

This repository contains the Python codes used for text cleaning, text augmentation and text classification and evaluation for invoice classification task. This is a combination of data augmentation with deep learning approaches to solve the invoice classsification task. Different augmentation size and approach paired with different classifiers will render different results. A key evaluation metric to consider is the accuracy and the macro-f1 score, where accuracy measures the 

## Data Source

Due to data privacy and large volume size of encoded dataset, there are no datasets in this repository. However, it is straightforward to create a sample dataset. A dataset with two columns - 'description' which contains the invoice text, and 'label' which contains the invoice category is required to be used together with the codes below.

## Text Cleaning

For text cleaning, refer to 'invoice-text-classification/text_cleaning'
Text cleaning includes removal of digits, stopwords, symbols, single character, multiple spaces and lowering case of text.

Depending on the dataset type, more cleaning tasks may be required to improve the information retention within the short text, which in itself is a challenge given the limited semantic information.

For train-text split codes, refer to 'invoice-text-classification/train_test_split'

## Text Augmentation

There are four data augmentation techniques in this repository, namely semantic enrichment, WordNet lexicon substitution, GloVe embedding substitution and BERT embedding substitution. All four methods could be used to generate synthetic training data.

Refer to the links below for the codes.
'invoice-text-classification/semantic_enrichment'
'invoice-text-classification/wordnet_aug'
'invoice-text-classification/glove_aug'
'invoice-text-classification/bert_aug'

## Text Classification

There are three classifiers in this repository, namely LSVM, Bi-LSTM and BERT. Bi-LSTM and BERT are deep learning classifiers and considered state of the art while LSVM is a traditional text classifier. 

Refer to the links below for the codes.
'invoice-text-classification/lsvm'
'invoice-text-classification/bi-lstm'
'invoice-text-classification/bert'
