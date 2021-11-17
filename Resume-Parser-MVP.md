# Resume Parser Using NLP - MVP


### Goal of the Project
The purpose of this project is to parse information from a resume pdf files and resumes dataset to help job seekers to find the potential field according to their resumes contents.

### Exploratory Data Analysis
- Remove duplicates.
- Remove missing values (Empty TEXT).
- Romove unneeded columns which are PATH, Category and ID.
- Remove any resume with less than 100 words.
- Remove any word with less than 3 characters.

before applying EDA, we were had **5828** rows collected from four different datasets and **2789** after EDA.
### Natural Language Processing
- Verbs Lemmatisation 
- Remove English stopwords
- Remove domain specific stop words
- Remove extra white spaces, tabs and line breaks
- Remove any digits and all punctuations.
<br/><br/>
After all these previous steps the most frequent words are visualised as Word Cloud and Bar Chart:
### Data Visualisation
<img src="https://github.com/shhdSU/Resume_Parser_NLP/blob/main/Images/word_cloud_plot.png" width="500"/> <br/>
> Word Cloud

<img src="https://github.com/shhdSU/Resume_Parser_NLP/blob/main/Images/words_freq_plot.png" width="500"/> <br/>
> Bar Chart

<br/> For a next stage preparation, data vectorization applied.
### Data Vectorization
- Count Vectorizer Without grams.
- Count Vectorizer With binary grams.
- TF-IDF Vectorizer Without grams.
- TF-IDF Vectorizer With binary grams.


### Futrue Work
- Topic modeling and Data Clustering.
- More data visualisation.
