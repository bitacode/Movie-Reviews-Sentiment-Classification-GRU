# Sentiment Classification with GRU

## Introduction

A Gated Recurrent Unit (GRU) is a type of recurrent neural network (RNN) architecture that is used in the field of deep learning. GRUs are particularly effective for processing sequences of data for tasks like time series prediction, natural language processing, and speech recognition. They address some of the shortcomings of traditional RNNs, particularly issues related to long-term dependencies in sequence data.

Gated Recurrent Units were introduced as a solution to the vanishing gradient problem. GRUs use gating mechanisms to control the flow of information. These gates determine what information should be passed to the output and what should continue to be retained in the network's internal state, allowing the model to better capture dependencies for sequences of varied lengths.

## Dataset

This experiment employs a dataset that comprises movie reviews. The dataset used for model training is publicly available on Kaggle and accessible for free on the internet. The link to this data is [Kaggle Rotten Tomatoes EDA](https://www.kaggle.com/code/stefanoleone992/rotten-tomatoes-eda). The movie reviews were annotated using [RoBERTa](https://github.com/bitacode/Labeling-Dataset-For-Sentiment-Analysis.git).

## Results

The GRU model's training results indicate a training loss of 0.5820 with an accuracy of 0.7828, showing that the model is learning the patterns in the training data fairly well, with about 78% accuracy. On the validation set, the model achieved a lower validation loss of 0.5470 and a higher accuracy of 0.7985, suggesting that it generalizes well to unseen data and is not overfitting.


The GRU model achieved an overall accuracy of 80% across the dataset, with balanced precision, recall, and F1-scores of 0.80 each for both the macro and weighted averages. The model performs well in identifying positive and negative sentiments, achieving F1-scores of 0.85 and 0.83, respectively. However, it slightly underperforms on neutral sentiment, with a lower F1-score of 0.71, indicating some challenges in accurately distinguishing neutral cases.

## Prospect

GRU is specifically designed for sequential data, which allows it to perform well in sentiment analysis tasks. However, based on the training results, it’s clear that this experiment needs refinement to improve performance on neutral sentiment classifications. Increasing the number of epochs to 100 or more could further enhance the results.

