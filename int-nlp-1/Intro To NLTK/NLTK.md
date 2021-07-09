### Introduction to NLTK 

### 1. What is NLTK ❓

 NLTK (Natural Language Toolkit) is a suite that contains libraries and programs for statistical language processing. 
 It is one of the most powerful NLP libraries, which contains packages to make machines understand human language and reply to it with an appropriate response.
   
 It helps practitioners by providing easy-to-use interfaces to over 50 lexical and corpora resources, with text processing libraries for classification, tokenization, tagging, stemming, parsing, and semantic reasoning, wrappers for industrial-strength NLP libraries. The corpora of data consist of data from various applications over the internet; for text analytics, we can get data. By analyzing tweets on Twitter, we can find trending news and people’s reactions to a particular event. Amazon can understand user feedback or review on the specific product. 
 BookMyShow can discover people’s reviews about the movie, which can be both positive or negative. Youtube can also analyze and understand people’s viewpoints on a video.
 
Language is a method of communication with the help of which we can speak, read and write. Natural Language Processing (NLP) is the sub field of computer science especially Artificial Intelligence (AI) that is concerned about enabling computers to understand and process human language. We have various open-source NLP tools but NLTK (Natural Language Toolkit) scores very high when it comes to the ease of use and explanation of the concept. The learning curve of Python is very fast and NLTK is written in Python so NLTK is also having very good learning kit. NLTK has incorporated most of the tasks like tokenization, stemming, Lemmatization, Punctuation, Character Count, and Word count. It is very elegant and easy to work with.
   
 
  
  ### Image of NLTK and NLP what it does Exactly 
  ![image](https://user-images.githubusercontent.com/84801896/125044131-4c621500-e0b9-11eb-87a0-dee3614c2be1.png)
  
  ### image source:
  https://realpython.com/nltk-nlp-python/
  
### Natural Language Tool Kit (NLTK)
Among the above-mentioned NLP tool, NLTK scores very high when it comes to the ease of use and explanation of the concept. The learning curve of Python is very fast and NLTK is written in Python so NLTK is also having very good learning kit. NLTK has incorporated most of the tasks like tokenization, stemming, Lemmatization, Punctuation, Character Count, and Word count. It is very elegant and easy to work with.

### Why Learn Natural Langugae ToolKit ❓
The Natural language toolkit (NLTK) is a collection of Python libraries designed especially for identifying and tag parts of speech found in the text of natural language like English.The Natural Language Toolkit (NLTK) is a platform used for building Python programs that work with human language data for applying in statistical natural language processing (NLP). It contains text processing libraries for tokenization, parsing, classification, stemming, tagging and semantic reasoning.NLTK (Natural Language Toolkit) is a suite that contains libraries and programs for statistical language processing. It is one of the most powerful NLP libraries, which contains packages to make machines understand human language and reply to it with an appropriate response.

### NLTK FLash News
What this means is it gets everything related to a particular search query. Let’s say you want to try to get every piece of information regarding the hottest topic in the world today, COVID-19 or Coronavirus, you would specify so in the “query” parameter in the above function.
The “from_param” parameter and “to” parameter in the above function are the date parameters. It is asking you to specify the timeframe for which you want to get results for the search query. Since I mentioned, I want to get all results for a period of 30 days which is the maximum allowed timeframe for the free version, I will specify the from_param as the day 30 days before today’s date. However, I need to write this in a loop so that I can ensure I am getting every day.
### Top-quality data
Collect and annotate training data that meets and exceeds industry quality standards thanks to multiple quality control methods and mechanisms available in Toloka.
### Scalable projects
Have any amounts of image, text, speech, audio or video data collected and labeled for you by millions of skilled Toloka users across the globe.
### Cost-efficiency
Save time and money with this purpose-built platform for handling large-scale data collection and annotation projects, on demand 24/7, at your own price and within your timeframe.
### Free, powerful API
Build scalable and fully automated human-in-the-loop machine learning pipelines with a powerful open API and Python library for easy integration.




### Installing NLTK 
NLTK is one of the leading platforms for building Python programs that can work with human language data. 
It presents a practical introduction to programming for language processing. NLTK comes with a host of text processing libraries for 
sentence detection, tokenization, lemmatization, stemming, parsing, chunking, and POS tagging. 


NLTK provides easy-to-use interfaces to over 50 corpora and lexical resources. 
The tool has the essential functionalities required for almost all kinds of natural language processing tasks with Python.

### Installation
 * pip install nltk
 ![nltk installation](https://github.com/ManishaAnaparthi/Images/blob/460075d94db4c4249ee61ae325c5ff22ca3d8b5e/Screenshot%20(3).png)
 

### Features


*   Stemming
*   Recommendation
*   Sentiment analysis
*   Translation

  
   ### Getting started with NLTK
  Download NLTK –  you can download NLTK with nltk.download()
  ### Import NLTK
  You can import NLTK directly using import.
  ```
 import nltk
 ```

  Importing dataset from corpus
  Some simple operations with NLTK
  ### Tokenizing 
  Tokenizing means breaking down large words or sentences into smaller length form, which helps to clean the data for processing and classification.

  ### Tokenize words
  To tokenize words means to break down a sentence into an array of words.

  ### Tokenize sentences
  To tokenize sentences is to break down long sentences into parts that differ by breakpoints.

  ### Part of speech (POS)
  A part-of-speech tagger(POS-tagger) generally processes word-sequences; for each word, it attaches a part of speech. 
  The tokenization concept should be used to achieve this. (Tokenization is the process of dividing the quantity of text into smaller pieces called tokens.)
  
  ## What is Lemmatization?
   
Lemmatization technique is like stemming. The output we will get after lemmatization is called ‘lemma’, which is a root word rather than root stem, the output of stemming. After lemmatization, we will be getting a valid word that means the same thing.

NLTK provides WordNetLemmatizer class which is a thin wrapper around the wordnet corpus. This class uses morphy() function to the WordNet CorpusReader class to find a lemma. Let us understand it with an example 
   
   ### First, we need to import the natural language toolkit(nltk).
   
*  import nltk
*  nltk.download('wordnet')
*  from nltk.stem import WordNetLemmatizer
  
   

   ## Create WordNetLemmatizer object
*  wnl = WordNetLemmatizer()
  
*  ### Single word lemmatization examples
*  list1 = ['kites', 'babies', 'dogs', 'flying', 'smiling', 'driving', 'died', 'tried', 'feet']
*  for words in list1:
    print(words + " ---> " + wnl.lemmatize(words))
    
    ![7](https://user-images.githubusercontent.com/84801896/124072061-e98bd080-da5d-11eb-859b-361ad9183f44.PNG)
    
 ### What is Tokenizing?
 It may be defined as the process of breaking up a piece of text into smaller parts, such as sentences and words. These smaller parts are called tokens. For example, a word is    a token in a sentence, and a sentence is a token in a paragraph.

  As we know that NLP is used to build applications such as sentiment analysis, QA systems, language translation, smart chatbots, voice systems, etc., hence, in order to build     them, it becomes vital to understand the pattern in the text. The tokens, mentioned above, are very useful in finding and understanding these patterns. We can consider     tokenization as the base step for other recipes such as stemming and lemmatization.

### NLTK package
nltk.tokenize is the package provided by NLTK module to achieve the process of tokenization.

Tokenizing sentences into words
Splitting the sentence into words or creating a list of words from a string is an essential part of every text processing activity. Let us understand it with the help of various functions/modules provided by nltk.tokenize package.

### NLTK IMPLEMENTATION

(a) Import the NLTK module and download the text resources needed for the examples.

![image](https://antoiloui.com/images/blog/post-3/banner.jpg)  


(b) Take a sentence and tokenize into words. Then apply a part-of-speech tagger.

(c) get texts for corpus analysis

(d) find words with similar concordance to a given word

(e) plot where in the text certain words appear

(f) print the identity of a text, the length of the text and its vocabulary

(g) print some statistics of word occurrence in the text
  
