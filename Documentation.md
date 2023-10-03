# NLP Research Internship Assignment - Biomedical Text Analysis

Welcome to the solution for the NLP Research Internship Assignment focused on Biomedical Text Analysis. This repository contains the code and documentation for this assignment.

## Task 1: Data Extraction

### Chosen Topic: Artificial Intelligence in Healthcare

The chosen topic for this assignment is "Artificial Intelligence in Healthcare" due to its increasing importance in improving medical diagnosis, patient care, and research. This topic allows exploration of the latest developments in AI applications within the healthcare domain.

To extract relevant abstracts, the MEDLINE API was utilized to search for articles related to "Artificial Intelligence in Healthcare" and fetch their abstracts.

## Task 2: Advanced NLP Analysis

### General Keyword Extraction

Advanced NLP techniques were applied to extract keywords from the introduction sections of the abstracts. This involved the following steps:

- Tokenization: Tokenization of the text into words.
- Stopword Removal: Removal of common English stopwords to focus on meaningful keywords.
- TF-IDF Vectorization: Representation of words' importance using TF-IDF.
- Keyword Selection: Selection of the top 5 TF-IDF keywords for each abstract.

### Topic Modeling and Keyword Extraction

Latent Dirichlet Allocation (LDA) was used for topic modeling on the introduction sections of the abstracts. This involved the following steps:

- TF-IDF Matrix: Creation of a TF-IDF matrix for the introduction sections.
- LDA Model: Utilization of Latent Dirichlet Allocation with 30 topics based on the perplexity metric (explained below).
- Model Fitting: Fitting the LDA model to the TF-IDF matrix.
- Keyword Extraction: Extraction of the top 10 keywords for each topic.

## Task 3: Interpretation and Usefulness

The insights derived from these analyses provide valuable information for research. The keywords extracted from the introduction sections offer a concise summary of the key concepts in each abstract. The topics identified through LDA clustering can help categorize the abstracts based on their content.

These insights are useful for understanding trends and focus areas within the field of artificial intelligence in healthcare. They can assist in decision-making regarding research directions and collaborations.

## Task 4: Methodology

### Keyword Extraction Methodology

- Tokenization: Tokenization of the introduction sections.
- Stopword Removal: Removal of common English stopwords.
- TF-IDF Vectorization: Representation of words' importance using TF-IDF.
- Keyword Selection: Selection of the top 5 TF-IDF keywords for each abstract.

### Topic Modeling Methodology

- TF-IDF Matrix: Creation of a TF-IDF matrix for the introduction sections.
- LDA Model: Utilization of Latent Dirichlet Allocation with 30 topics based on the perplexity metric.
- Model Fitting: Fitting the LDA model to the TF-IDF matrix.
- Keyword Extraction: Extraction of the top 10 keywords for each topic.

### Perplexity - Choosing the Number of Topics

Perplexity, a topic modeling measure, assesses model prediction quality. Lower perplexity scores imply better performance.
In our analysis, increased topics correlated with rising perplexity scores, indicating reduced benefits. Occasional perplexity drops did not signify significantly improved models.
The choice of 30 topics resulted from practicality and the absence of a clear "elbow" point in the perplexity graph

### Further Enhancements
To bolster topic modeling:

- Experiment more with model hyperparameters.
- Scrutinize data quality for noise reduction.
- Emphasize effective interpretation of existing topics.
- Explore alternate topic modeling algorithms like Non-Negative Matrix Factorization (NMF).
