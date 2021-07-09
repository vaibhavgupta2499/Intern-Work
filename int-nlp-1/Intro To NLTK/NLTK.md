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

![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/installation.PNG)  


(b) Take a sentence and tokenize into words. Then apply a part-of-speech tagger.

![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/TOKENIZER%20INSTALL.PNG)  

(c) From the tagged words, identify the proper names

![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/identifying%20names.PNG) 

(d) Get texts for corpus analysis

![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/text%20corpus.PNG) 

(e) Find words with similar concordance to a given word

![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/similar%20words.PNG) 

(f) Plot where in the text certain words appear

![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/lexical%20dispersion.PNG) 

(g) Print the identity of a text, the length of the text and its vocabulary

![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/length%20text.PNG) 

(h) Print some statistics of word occurrence in the text
 
![image](https://github.com/PranavKapoor28/Intern-Work/blob/main/int-nlp-1/Intro%20To%20NLTK/Images/occurance%20statistics.PNG) 


### Named entity recognition (NER),

Named entity recognition (NER), or named entity extraction is a keyword extraction technique that uses natural language processing (NLP) to automatically identify named entities within raw text and classify them into predetermined categories, like people, organizations, email addresses, locations, values, etc.

A simple example:

![image](https://user-images.githubusercontent.com/84801896/125066162-4deb0780-e0d0-11eb-8800-3549eac2b2f0.png)
 Using NER, you can automate endless tasks, with almost no human intervention.
 ### How to Do Named Entity Recognition with Python
 
 MonkeyLearn is a SaaS platform with an array of pre-built NER tools and SaaS APIs in Python, like person extractor, company extractor, location extractor, and more.
 
 ### 1. Install MonkeyLearn Python SDK
 The API tab shows how to integrate using your own Python code (or Ruby, PHP, Node, or Java). We’ll start performing NER with MonkeyLearn’s Python API for our pre-built company extractor. The API will access the extractor automatically:
 
 ![image](https://user-images.githubusercontent.com/84801896/125066448-a4584600-e0d0-11eb-8403-df4795a10cd4.png)


You can send plain requests to the MonkeyLearn API and parse the JSON responses yourself, but MonkeyLearn offers easy integration with SDKs in a number of languages. 

Sign up to get your API key then download and install the Python SDK:

 ```
 pip install monkeylearn
 ```
 
### 2.Run your NER model
Now that you're set up, enter the below to start running MonkeyLearn’s NER analysis:
 ```
rom monkeylearn import MonkeyLearn

ml = MonkeyLearn('<<Your API key here>>')
model_id = 'ex_A9nCcXfn'
data = ['first text', {'text': 'SpaceX is an aerospace manufacturer and space transport services company headquartered in California. It was founded in 2002 by entrepreneur and investor Elon Musk with the goal of reducing space transportation costs and enabling the colonization of Mars.', 'external_id': 'ANY_ID'}, '']
response = ml.extractors.extract(model_id, data=data)

print(response.body)
```
### 3. Output your model
The output will be a Python dict generated from the JSON sent by MonkeyLearn – in the same order as the input text – and should look something like this:

```
[
    {
        'text': 'first text', 
        'external_id': None, 
        'error': False, 
        'extractions': []
     }, {
        'text': 'SpaceX is an aerospace manufacturer and space transport services company headquartered in California. It was founded in 2002 by entrepreneur and investor Elon Musk with the goal of reducing space transportation costs and enabling the colonization of Mars.', 
        'external_id': 'ANY_ID', 
        'error': False, 
        'extractions': [{
            'tag_name': 'COMPANY', 
            'extracted_text': 'SpaceX', 
            'parsed_value': 'SpaceX', 
            'count': 1
        }]
    }, {
        'text': '', 
        'external_id': None, 
        'error': True, 
        'error_detail': 'Invalid text, empty strings are not allowed', 
        'extractions': None
    }
]
```
### Now you’re set up to perform NER automatically. You can change the models to try out something new or create your own model, then call it with Python.












### SUMMARIZATION

![image](https://user-images.githubusercontent.com/84801896/125067709-3b71cd80-e0d2-11eb-8ded-0674098d0ec7.png)

### image source :https://realpython.com/python-nltk-sentiment-analysis/
* Natural Language Toolkit
NLTK is a leading platform for building Python programs to work with human language data. It provides easy-to-use interfaces to over 50 corpora and lexical resources such as WordNet, along with a suite of text processing libraries for classification, tokenization, stemming, tagging, parsing, and semantic reasoning, wrappers for industrial-strength NLP libraries, and an active discussion forum.

* Thanks to a hands-on guide introducing programming fundamentals alongside topics in computational linguistics, plus comprehensive API documentation, NLTK is suitable for linguists, engineers, students, educators, researchers, and industry users alike. NLTK is available for Windows, Mac OS X, and Linux. Best of all, NLTK is a free, open source, community-driven project.

* NLTK has been called “a wonderful tool for teaching, and working in, computational linguistics using Python,” and “an amazing library to play with natural language.”

* Natural Language Processing with Python provides a practical introduction to programming for language processing. Written by the creators of NLTK, it guides the reader through the fundamentals of writing Python programs, working with corpora, categorizing text, analyzing linguistic structure, and more. The online version of the book has been been updated for Python 3 and NLTK 3. 






  

