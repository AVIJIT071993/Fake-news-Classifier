# Fake-news-Classifier
The aim of the project to classify news as real or fake. We have 6335 rows of data, which have a title and text of the news. Feature scaling is done with the help of TfidVectorizer. The data is trained on PassiveAggressiveClassifier. 

Data scraping is done with the help of beautifulsoup and request. The data is scrapped from "inshorts". They are then feature engineered and feed into the model. In the output, news are classified as real or fake.

Python Libraries Required:
1. pip install numpy
2. pip install pandas
3. pip install seaborn
4. pip install scikit-learn
5. pip install beautifulsoup4
6. pip install urllib3
7. pip install python-csv

TfidfVectorizer:
TFIDF, short for term frequency–inverse document frequency, is a numerical statistic that is intended to reflect how important a word is to a document in a collection or corpus.[1] It is often used as a weighting factor in searches of information retrieval, text mining, and user modeling. The tf–idf value increases proportionally to the number of times a word appears in the document and is offset by the number of documents in the corpus that contain the word, which helps to adjust for the fact that some words appear more frequently in general.

Term Frequency (TF)
The number of times a word appears in a document divded by the total number of words in the document. Every document has its own term frequency.
               /  N \ 
i d f(w) = log |----| 
               |d f | 
               \   t/ 


Inverse Data Frequency (IDF)
The log of the number of documents divided by the number of documents that contain the word w. Inverse data frequency determines the weight of rare words across all documents in the corpus.

The TF-IDF is simply the TF multiplied by IDF.
