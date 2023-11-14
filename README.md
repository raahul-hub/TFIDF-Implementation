# TFIDF-Implementation

# TF-IDF (Term Frequency-Inverse Document Frequency)

TF-IDF is a numerical statistic that reflects the importance of a word in a document relative to a collection of documents (corpus). It is commonly used in information retrieval and text mining.

## Term Frequency (TF)

Term Frequency measures how often a term (word) appears in a document. It is calculated as the number of times a term appears in a document divided by the total number of terms in that document.

\[ \text{TF}(t, d) = \frac{\text{Number of times term \(t\) appears in document \(d\)}}{\text{Total number of terms in document \(d\)}} \]

## Inverse Document Frequency (IDF)

Inverse Document Frequency measures how important a term is across the entire corpus. Terms that appear in many documents will have a lower IDF, while terms that appear in fewer documents will have a higher IDF.

\[ \text{IDF}(t, D) = \log\left(\frac{\text{Total number of documents in the corpus \(N\)}}{\text{Number of documents containing term \(t\) + 1}}\right) \]

(Note: Adding 1 to the denominator is a smoothing technique to avoid division by zero.)

## TF-IDF

The TF-IDF score for a term \(t\) in a document \(d\) is the product of TF and IDF:

\[ \text{TF-IDF}(t, d, D) = \text{TF}(t, d) \times \text{IDF}(t, D) \]


Lets implement this with Python



