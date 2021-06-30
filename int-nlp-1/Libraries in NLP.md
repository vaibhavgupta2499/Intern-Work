### Libraries in NLP

Natural Language Processing(NLP), a field of AI, aims to understand the semantics and connotations of natural human languages. It focuses on extracting meaningful information from text and train data models based on the acquired insights. The primary NLP functions include text mining, text classification, text analysis, sentiment analysis, word sequencing, speech recognition & generation, machine translation, and dialog systems, to name a few. 
Thanks to the development of useful NLP libraries, today, NLP is finding applications across the various parallels of the industrial landscape. In fact, NLP has now become an integral part of Deep Learning development. Extracting valuable information from free text is essential for developing chatbots, patent research & analysis, voice/speech recognition, patient data processing, and querying image content, among other use cases of NLP.
The fundamental aim of NLP libraries is to simplify text preprocessing. A good NLP library should be able to correctly convert free text sentences into structured features (for example, cost per hour) that can easily be fed into ML or DL pipelines. Also, an NLP library should have a simple-to-learn API, and it must be able to implement the latest and greatest algorithms and models efficiently. 
Although there are numerous NLP libraries designed for specific NLP applications, today, we’re going to draw a comparison of the functions of the top NLP libraries in Python. 


Now, let’s dive into the discussion about the top NLP libraries!



1. Natural Language Toolkit (NLTK)
2. Gensim
3. CoreNLP
4. spaCy
5. TextBlob



### 1.Natural Language Toolkit (NLTK)
NLTK is one of the leading platforms for building Python programs that can work with human language data. 
It presents a practical introduction to programming for language processing. NLTK comes with a host of text processing libraries for 
sentence detection, tokenization, lemmatization, stemming, parsing, chunking, and POS tagging. 


NLTK provides easy-to-use interfaces to over 50 corpora and lexical resources. 
The tool has the essential functionalities required for almost all kinds of natural language processing tasks with Python.

### Installation
 * pip install nltk
 

### Features


*   Stemming
*   Recommendation
*   Sentiment analysis
*   Translation


### 2.Gensim
Gensim is a Python library designed specifically for “topic modeling, document indexing, and similarity retrieval with large corpora.”
All algorithms in Gensim are memory-independent, w.r.t., the corpus size, and hence, it can process input larger than RAM. With intuitive interfaces, Gensim allows for efficient multicore implementations of popular algorithms, including online Latent Semantic Analysis (LSA/LSI/SVD), Latent Dirichlet Allocation (LDA), Random Projections (RP), Hierarchical Dirichlet Process (HDP) or word2vec deep learning. 


Gensim features extensive documentation and Jupyter Notebook tutorials. It largely depends on NumPy and SciPy for scientific computing. 
Thus, you must install these two Python packages before installing Gensim.

  * Gensim is an open-source vector space and topic modelling toolkit.
  * Gensim uses numpy and sciPy.
  * Gensim is designed for data stemming ,habdle large text collections and efficient incremental algorithms.
  
 ### Installation
  
  * pip install gensim

 
 ### Features
  
  * FastText
  * Word2Vec
  * Latent Semantic Analysis 
  * Latent dirichlet Allocation
  * tf-idf ( Term frequency-inverse document frequency)



### 3. CoreNLP
Stanford CoreNLP comprises of an assortment of human language technology tools. It aims to make the application of linguistic analysis tools to a piece of text easy and efficient. With CoreNLP, you can extract all kinds of text properties (like named-entity recognition, part-of-speech tagging, etc.) in only a few lines of code. 

Since CoreNLP is written in Java, it demands that Java be installed on your device. However, 
it does offer programming interfaces for many popular programming languages, including Python. 
The tool incorporates numerous Stanford’s NLP tools like the parser, sentiment analysis, bootstrapped pattern learning, part-of-speech (POS) tagger, 
named entity recognizer (NER), and coreference resolution system, to name a few. Furthermore, CoreNLP supports four languages apart from 
English – Arabic, Chinese, German, French, and Spanish.

### Installation
  * pip install stanford-corenlp
 
### Features
  * Lemmatization
  * Part-Of-Speech Tagging
  * Morphological Tagging
  * Named ENtity Recognition
  * Tokenization
  * Sentence Splitting

  

### 4.spaCy

spaCy is an open-source NLP library in Python. It is designed explicitly for production usage – it lets you develop applications that process and understand huge volumes of text.  

spaCy can preprocess text for Deep Learning. It can be be used to build natural language understanding systems or information extraction systems. 
spaCy is equipped with pre-trained statistical models and word vectors. It can support tokenization for over 49 languages. 
spaCy boasts of state-of-the-art speed, parsing, named entity recognition, convolutional neural network models for tagging, and deep learning integration.


### Installation
  * pip install -U spacy

### Features
  * Tokenization
  * POS Tagging 
  * Dependency Parsing
  * Lemmatization
  * Sentence Boundary Detection
  * Named Entity Recognition
  * Entity Linking
  * Text Classification
  * Similarity
  


### 5.TextBlob

TextBlob is a Python (2 & 3) library designed for processing textual data. It focuses on providing access to common text-processing operations through familiar interfaces. TextBlob objects can be treated as Python strings that are trained in Natural Language Processing.

TextBlob offers a neat API for performing common NLP tasks like part-of-speech tagging, noun phrase extraction, sentiment analysis, classification, language translation, 
word inflection, parsing, n-grams, and WordNet integration.
### Installation
 
   * pip install -U tectblob
   * python _m textblob.download_corpora
  
### Features
   * Tokenization
   * Parsing
   * Spelling Corrrection
   * Sentiment Analysis
   * Part-Of_Speech tagging
   * n-grams
   * Translation
   * word & phrase frequencies
   

### 6.Pattern

Pattern is a text processing, web mining, natural language processing, machine learning, and network analysis tool for Python. It comes with a host of tools for data mining (Google, Twitter, Wikipedia API, a web crawler, and an HTML DOM parser), NLP (part-of-speech taggers, n-gram search, sentiment analysis, WordNet), 
ML (vector space model, clustering, SVM), and network analysis by graph centrality and visualization. 
### Installation
 
   * pip install pattern
  
