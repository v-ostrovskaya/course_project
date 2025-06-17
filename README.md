Knowledge Tree: Extracting Concepts from Natural Language Texts Using Complex Networks
This project presents an automated, unsupervised framework for extracting and organizing concepts from natural language texts. The primary focus is on low-resource languages, with Afrikaans selected as the pilot case.

Project Objectives
Atomic Concept Extraction: Identify minimal semantic units through lemmatization and entity normalization.

Semantic Clustering: Group concepts by distributional similarity using Word2Vec embeddings.

Knowledge Graph Construction: Build interpretable relationships between clusters using graph-based methods.

Motivation
Afrikaans, spoken by 14–21 million people, has very limited pretrained NLP resources compared to English. This project addresses this gap by building a flexible proto-knowledge tree for semantic visualization without the need for labeled data.

Approach
Corpus: Autshumato Monolingual Afrikaans Corpus v2.1 (1.19M segments, 20.2M tokens, government/legal texts)

Preprocessing: Tokenization, lemmatization (using Stanza), substitution of proper nouns and numbers, stopword removal

Embedding: Skip-gram Word2Vec (vector_size=100, window=5)

Clustering: PCA for dimensionality reduction, KMeans clustering (k=10)

Visualization: Cluster graph construction and interpretation using matplotlib

Error Analysis: Validation with native speakers

Novelty
First integrated end-to-end framework for concept extraction in Afrikaans

Combines Word2Vec embeddings with graph-based clustering

Requires no labeled data

Tailored preprocessing for language-specific features such as double negation and phonetic orthography

Future Work
Integration of POS-aware disambiguation in preprocessing

Fine-tuning transformer models (e.g. AfriBERTa) for improved embeddings

Extension to other low-resource languages like isiZulu and Sesotho

References
Key sources include works on Word2Vec, GloVe, fastText, Stanza, and studies on NLP for Afrikaans. See the presentation references for full details.

Data
Download the final .npy file with the embeddings: Yandex Disk link
