# Resume Parser Using NLP - MVP


#### Goal of the Project
> The purpose of this project is to parse information from a resume pdf files and resumes dataset to help job seekers to find thier potential field according to thier resumes contents.

#### Exploratory data analysis
- found duplicate resumes and removed it.
- found any missing values and removed it.
- Romoved unneeded columns which are PATH and Category.
- removed any resume with less than 100 words.
- removed any word with less than 3 characters.

</br>
before EDA procedures we had 5828 rows collected from four datasets and after that it becomes 2789 row of resumes

#### Natural Language Processing
</br>

>  NLP Includes:
- Lemmatized verbs in list of tokenized words
- Removed English stopwords
- Removed domain specific stop words
- Removed extra spaces, tabs, and line breaks
- Removed digits and all punctuations.

 ##### After all these steps of processing and cleaning we visualised and vectorized the data which incloudes:
##### Data Visualisation
> Word Cloud Plot
<img src="https://github.com/Wafaa-Alharbi/Resume-Parser-NLP/blob/main/Images/word_cloud_plot.PNG" width="500"/> 

> Most Frequent Words Plot
<img src="https://github.com/Wafaa-Alharbi/Resume-Parser-NLP/blob/main/Images/words_freq_plot.PNG" width="500"/> 

##### Data Vectorization
- Count Vectorizer Without grams.
- Count Vectorizer With binary grams.
- TF-IDF Vectorizer Without grams.
- TF-IDF Vectorizer With binary grams.


#### Futrue Work
- We will apply Topic modeling and clustering into the data.


