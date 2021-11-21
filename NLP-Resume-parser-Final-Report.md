# Resume Parser Using Natural Language Processing Final Report 

### 
## Abstract
The purpose of this project is to use the power of Natural Language Processing to parse information from a resume pdf files.   

### Design
In order to parse resumes information, data was downloaded from different data resources.
Then, EDA, topic modeling and multiple classification models were implemented to get the best resluts.

## Data
- ### PDF Files
  The First dataset is __4,440__ resumes pdf files comes from  [Kaggle](https://www.kaggle.com/aishikai/resume-dataset?select=pdf) and 
  [GitHub](https://github.com/JAIJANYANI/Automated-Resume-Screening-System) , and after text extraction and intial cleaning, the resume texts and thier path converted into dataframe with __1,534__ rows and __2__ columns, which are:
  - TEXT Columns contains resumes (one resume in each row).
  - PATH Columns contains the path of each resume.
- ### Ready Dataset
  These datasets comes from [Kaggle - resumes](https://www.kaggle.com/maitrip/resumes) and [Kaggle - ResumeDataSet](https://www.kaggle.com/dhainjeamita/resumedataset) and after combining them __1,388__ rows and __4__ columns are result, but all columns are dropped except __TEXT__ column to convert them into an unsupervised learning dataset, and after cleaning the number of rows becomes __1,255__.
  
#### Cleaning:
- Drop unneeded columns.
- Handle nulls.
- Handle Duplicates.
- English resumes only.
- Limitted to resumes that have more than 100 words and each word more than 3 characters.

#### Data visualisation and vectorization
- __visualisation:__ 
> Drew many graphs for understanding the data.
- __vectorization:__
1. Count Vectorizer Without grams.
2. Count Vectorizer With binary grams.
3. TF-IDF Without grams.
4. TF-IDF With binary grams.

#### NLP:
> NLP procedures done into multiple itreations

1- __Text Cleaning:__
- Remove english stop words.
- Remove domain specific stop words (in separated multiple time).
- Lemmatization.
- Remove Entities.
- Remove any digits or special characters.

2- __Topic Modeling__:
> after trying many models we chose NMF with TF-IDF.
- For PDF files Dataset: 11 topics were chosen, which are : (Finance, Hospitality, Electrical and Mechanical Engineering, Sales and Marketing, Beauty Artist,  Secretarial, Accounting, Health, Accounting, Investment, Others)
- For ready Dataset: 13 topics were chosen, which are: ( Business Administration, Sales and Marketing, Accounting, Management Information System , Risk Management , Law, Hospitality, Electrical and Mechanical Engineering, Health, Graphics Design, Finance, Teaching, Development)

> after the topic modeling we merage the two datasets into one for next stage...

#### Classification:
> 7 models were tried and played with to get the best model that goes hand in hand with the dataset. 
After performing simple train and validation on the 7 models one was chosen for further investigation.
The implemented models:

<img src="https://github.com/Wafaa-Alharbi/Resume-Parser-NLP/blob/main/Images/classification_for_nlp_projet.png" width="500"/> <br/>


The best model was Decision Tree Classifier.
### Tools
- __Data manipulation and cleaning:__ Pandas and Numpy, Matplotlib
- __Data Storing:__ Sqlite3 and pickle
- __Text precossing:__ NLTK, spaCy, gensim, scikit-learn , pyPDF2
- __Topic Modeling:__ NMF (Non-negative Matrix factorization), LDA (Latent Derilicht Analysis)
- __Visualization:__ Tableau, matplotlib, seaborn
