# Resume Parser Using Natural Language Processing


### Introduction
Finding a job  is considered one of the major activities for humans. The purpose of this project is to use the power of Natural Language Processing to parse information from a resume pdf files, find the keywords, cluster them onto sectors based on their keywords, in order to help job seekers to find thier potential field according to thier resumes contents.

### Data Description
The dataset is 4440 resumes pdf files comes from  [Kaggle](https://www.kaggle.com/aishikai/resume-dataset?select=pdf) and 
[GitHub](https://github.com/JAIJANYANI/Automated-Resume-Screening-System) , and after text extraction and intial cleaning, the resume texts and thier path converted into dataframe with 1534 rows and 2 columns, which are:
- TEXT Columns contains resumes (one resume in each row).
- PATH Columns contains the path of each resume.


### Tools Description
- Data manipulation and cleaning: Pandas and Numpy
- Data Storing: Sqlite3 and pickle
- Text precossing: NLTK, spaCy, gensim, scikit-learn
- Topic Modelling: NMF (Non-negative Matrix factorization), LDA (Latent Derilicht Analysis)
- Visualization: Tableau, matplotlib, seaborn
- Other Python libraries or tools if needed 
