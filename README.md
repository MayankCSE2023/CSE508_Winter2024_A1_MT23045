# CSE508_Winter2024_A1_MT23045

# Information Retrieval Assignment Report

## Introduction

The aim of this assignment was to implement Information Retrieval (IR) techniques on a dataset of text files. The tasks included preprocessing the text, creating an inverted index, and executing queries using boolean operations. Additionally, positional indexing was implemented for more advanced queries.

## Methodology

### Text Preprocessing

The text preprocessing phase involved several steps:
- Lowercasing the text
- Removing ellipses and words with apostrophes attached
- Tokenization using NLTK's word_tokenize
- Removing stopwords and punctuation
- Joining the tokens back into a string

### Inverted Indexing

A unigram inverted index was created to map terms to the documents they appeared in. The index was stored using the pickle module for efficient loading.

### Boolean Query Execution

Boolean query execution was implemented with support for AND, OR, NOT, AND NOT, and OR NOT operations. The queries were processed by combining terms and operators, then executing the corresponding operations on the inverted index.

### Positional Indexing

To support more complex queries involving phrase structures, positional indexing was implemented. This involved recording the positions of terms in documents and checking their sequential relationships during query execution.

## Implementation

The code was implemented in a Jupyter notebook using Python. Key libraries utilized include NLTK for text processing and pickle for storing and loading indexes.

## Results

### Inverted Index

The inverted index was successfully created, and the first few entries were printed for verification.

### Boolean Query Execution

Sample queries were processed using the inverted index, and the results were displayed, including the query text, the number of documents retrieved, and their names.

### Positional Indexing

A positional index was created to support phrase queries. The first few entries of the positional index were printed, and sample phrase queries were executed.

## Discussion

### Strengths

- The implemented system successfully handles basic and complex queries.
- The preprocessing steps effectively clean the text data for better indexing.

### Weaknesses

- The current implementation assumes perfect preprocessing, and variations in user queries might lead to unexpected results.


## Conclusion

The implemented Information Retrieval system demonstrates effectiveness in handling various types of queries on a text dataset. The combination of boolean and positional indexing techniques allows for a versatile search functionality.

## Acknowledgments

- NLTK library for text processing functionality.
- Colab for providing a convenient platform for development.

## References

- NLTK documentation: [link](https://www.nltk.org/)
- Colab: [link](https://colab.research.google.com/)

