# Project Name: Movie Genres Classification

## Introduction
Welcome to the Movie Genres Classification project! This project aims to predict movie genres based on their overviews. Accurate movie genre prediction enhances user experience and refines content recommendations in modern entertainment platforms.

## Dataset
- **Source**: IMDB Movie Dataset
- **Size**: 41k movies
- **Unique Genres**: 27
- **Average Genres per Movie**: 3
- **Split**: 
  - Training data: 70%
  - Development data: 10%
  - Test data: 20%

## Data Pre-processing
Steps involved in pre-processing the text data:
1. Convert text to lowercase
2. Remove punctuations
3. Remove stop-words
4. Apply stemming
5. Tokenization

## Word Embeddings
Methods used for word embeddings:
- Bag of Words
- TF-IDF
- BERT Tokenizer
- GloVe
- Word2Vec

## Classification Methods
The following methods are used for classifying movie genres:
- Logistic Regression (Baseline)
- Naïve Bayes
- Random Forests
- SVM
- DistilBERT using BERT Tokenizer

### Multi-Label Adaptation
- **Multioutput Classifier**: Fits one classifier per target.
- **Label Powerset**: Transforms a multi-label problem into a multi-class problem with one multi-class classifier trained on all unique label combinations.

## Evaluation Metrics
- Accuracy
- Weighted average F1-score

## Key Findings
- Static word embeddings have limitations in extracting meaningful information.
- DistilBERT addresses word ambiguity effectively and accounts for the effect of all words in a sentence.

## Challenges
- Dataset issues: Sparsity, imbalance
- Classification issues: Computational complexity, label ambiguity, feature dimensionality, inter-class variability
