---
title: Sentiment Analysis
date: 2021-03-10T13:13:47.650Z
summary: Used GloVe pre-trained vector embeddings in PyTorch to perform sentiment analysis on text data utilizing binary classification.
draft: false
featured: false
tags:
  - ml
external_link: ""
links:
  - url: https://github.com/pollmix/sentiment-analysis
    name: Link
    icon_pack: fab
    icon: github
image:
  filename: ""
  focal_point: Smart
  preview_only: false
---

This model will predict the sentiment of a given sentence. If the sentence is positive the result values will be close to zero otherwise if it's a negative sentence then the result will be close to one.

```
INPUT: A single sentence
I hate that show

OUTPUT: value close to 0 means positive, close to 1 means negative sentiment
0.8913049101829529
```

### Tools Used

- Python
- PyTorch
- Matplotlib
- spaCy
- pandas
- scikit-learn
- seaborn

### Concepts covered

- Feature extraction
- Numericalization
- Encoding strategies
- Embedding
- Classification
- RNN (Recurrent Neural Network)
- One-hot encoded tensors

### Details

We represented text data as features for machine learning. We performed different techniques like numericalize text data, one-hot encoding, count and frequency-based encodings, and probability-based embeddings. We explored machine learning algorithms, such as gloVe and word2vec, can be used to generate low dimensionality embeddings which capture meaning, as well as semantic relationships that exist in text data.

GloVe pretrained vector embeddings are freely available for us to use in PyTorch, and we saw how we could construct analogies and find neighboring words using these embeddings. We then use these gloVe pretrained word vectors to perform sentiment analysis on text data. This is essentially a binary classification problem. Along the way, we studied some optimizations that we could apply to our recurrent neural networks such as multi-layer RNNs and bidirectional RNNs.
