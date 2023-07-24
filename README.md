# Semantic Enrichment, Data Augmentation and Deep Learning for Invoice Text Classification: A Novel Strategy

This repository contains the Python codes used for text cleaning, semantic enrichment, text augmentation and text classification and evaluation for invoice classification task. This is a combination of semantic enrichment and data augmentation with deep learning approaches to solve the invoice classsification task. Different augmentation size and approach paired with different classifiers will render different results. A key evaluation metric to consider is the accuracy and the macro-f1 score, given the multi-class labels which introduces severe class imbalance within the invoice text data class distribution. 

## Data Source

Due to data privacy and large volume size of encoded dataset, there are no datasets in this repository. However, it is straightforward to create a sample dataset. A dataset with two columns - 'description' which contains the invoice text, and 'label' which contains the invoice category is required to be used together with the codes below.

## Text Cleaning

For text cleaning, refer to 'invoice-text-classification/text_cleaning'.
Text cleaning includes removal of digits, stopwords, symbols, single character, multiple spaces, lowering case of text and retaining only English words.
  
Depending on the dataset type, more cleaning tasks may be required to improve the information retention within the short text, which in itself is a challenge given the limited semantic information.
  
For train-text split codes, refer to 'invoice-text-classification/train_test_split'

## Semantic Enrichment

For semantic enrichment, refer to 'invoice-text-classification/semantic_enrichment'. Semantic enrichment of the text is based on auxiliary information from the label text.

## Text Augmentation

There are three data augmentation techniques in this repository, namely lexical synonym replacement (WordNet), Word Embedding similar word replacement (GloVe), and Contextual Word Embedding word replacement (BERT). All three methods could be used to generate synthetic training data.
  
Refer to the links below for the codes:  
'invoice-text-classification/wordnet_aug'  
'invoice-text-classification/glove_aug'  
'invoice-text-classification/bert_aug'  

## Text Classification

There are three classifiers in this repository, namely LSVM, Bi-LSTM and BERT. Bi-LSTM and BERT are deep learning classifiers and considered state of the art while LSVM is a traditional text classifier. 
  
Refer to the links below for the codes:  
'invoice-text-classification/lsvm'  
'invoice-text-classification/bi-lstm'  
'invoice-text-classification/bert'  
