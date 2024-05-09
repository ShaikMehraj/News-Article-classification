# News-Article-classification

1. Count Vectorization

Concept:

Count vectorization is a fundamental approach that represents a document as a vector of word counts.
It focuses on the frequency of words appearing in a document, ignoring word order and semantics.
Process:

Tokenization: The text is split into individual words or tokens.
Vocabulary Building: A vocabulary containing all unique words across the entire corpus (collection of documents) is created.
Vectorization: Each document is represented as a vector of size equal to the vocabulary size. The value at each position in the vector represents the count of the corresponding word in the document.


2. Doc2Vec

Concept:

Doc2Vec is a more sophisticated technique that learns a fixed-length vector representation (embedding) for each document.
This vector captures not only word frequencies but also semantic relationships between words within the document.
Process:

Doc2Vec uses machine learning algorithms like Distributed Memory (DM) or Paragraph Vector (PV) to learn document embeddings.
These algorithms train a model to predict surrounding words or document context based on a given document.
During training, documents and the words within them are represented as vectors, and the model aims to minimize the distance between similar documents/words in the vector space.


3. TF-IDF Vectorizer:

Concept: Builds upon Count Vectorization by addressing the issue of high-frequency words dominating the representation. It considers both term frequency (TF) and inverse document frequency (IDF).

TF measures how often a word appears in a document.
IDF reflects how important a word is for a specific document compared to the entire corpus. Words that appear frequently across all documents will have lower IDF values.
Process:

Similar tokenization and vocabulary building as Count Vectorization.
TF-IDF score is calculated for each word in each document.
Each document is represented as a vector where each element represents the TF-IDF score for the corresponding word in the vocabulary.