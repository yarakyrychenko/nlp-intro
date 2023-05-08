# Intro to NLP (pre-transformers)

https://drive.google.com/drive/folders/1lVRHX5XNEL90ieV8_7BP4fT1gPrxcQsQ?usp=sharing

### Basics of sentiment analysis 

Sentiment analysis aims to determine the affective state — something more persistent than an emotion and less persistent than a mood — of a particular text. There are two broad ways of approaching the task:  

👉 Dictionaries: using lists of words grouped by categories. We count how many words from a category are in a text to determine its sentiment. Some well-validated dictionaries include Harvard General Inquirer 4, LIWC, and VADER.

Pros: simple, fast, transparent, lower risk of overfitting. 
Cons: sensitive to dictionary choice and scoring systems, don’t get sarcasm, high risk of underfitting.
 
👉 Classifiers: using machine learning techniques to determine sentiment. Usually, you would either need to have labeled data (ie some of your text items would need to be labeled by a human as belonging to a category), or use a model pre-trained by someone else. Some suitable models include Naive Bayes, Support Vector Machine, k-nearest neighbors, and neural nets.

Pros: pick up on nuances and get better results, don’t need to compile a dictionary.
Cons: may need labeled data, less transparent, can be time-consuming to train, higher risk of overfitting.

In psychology, we prefer dictionaries over classifiers because that way it’s easier to relate the sentiment to psychological phenomena we’re studying as opposed to the quirks of the model. Additionally, classifiers can be way more costly since specialized categories require new human-labeled samples. It’s usually easier to creat a new dictionary with the necessary category (like moral emotional words, words expressing temptation, etc). 
