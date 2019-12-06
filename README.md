# Toxic Comment Classification

The purpose of this project is to perform binary classification on natural language to determine if it is safe or unsafe in nature.

## Data Processing

This project uses a combination of two Kaggle competition datasets, namely:

1. [Jigsaw Toxic Comment Classification Challenge](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)
2. [Jigsaw Unintended Bias in Toxicity Classification](https://www.kaggle.com/c/jigsaw-unintended-bias-in-toxicity-classification)

In total these datasets consisted of around 2 million internet comments from a variety of sources, with around 10% of this data classified as unsafe. The two datasets were cleaned, and recombined and then balanced out to form a [new unbiased dataset](data.csv), which consists of around 360,000 comments with a 50/50 balance between safe and unsafe classes.

## Classification

Four different models were experimented with in this project

- Random Forests
- Logistic Regression
- Multilayer Perceptron
- Deep Learning

The results of these techniques were then compared. Additionally a few natural language processing (NLP) techniques were applied to some of the models. These NLP techniques consisted of the following,

- Alphanumeric tokens only
- Stopword removal
- Nouns only

## Results

The following table summarizes the results achieved by the best models from each model category.

| Method              | Accuracy | Precision | Recall   |
| ------------------- | -------- | --------- | -------- |
| Random Forests      | 0.854074 | 0.854281  | 0.854085 |
| Logistic Regression | 0.870507 | 0.871464  | 0.870392 |
| Deep Learning       | 0.890919 | 0.891543  | 0.891011 |
