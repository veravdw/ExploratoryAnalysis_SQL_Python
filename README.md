
# Mental Health Questionnaire Analysis 

The data for this analsysis comes from a survey held amongst tech employees, containing questions about their mental health. 
The survey was held in 5 different years, between different age groups and in different countries. 
This project is an exploratory analysis, aiming to get first insights into the answer data and the sample. 

## Format

The analysis is performed in a Jupyter notebook, and can be opened in any IDE that supports Jupyter notebook files (.ipynb).

## Dataset 

The dataset can be found via this url: https://www.kaggle.com/datasets/anth7310/mental-health-in-the-tech-industry 
and comes in the form of a .SQLITE file, containing 3 different tables with question, answer and survey data respectively.
The data can be queried using SQL (sqlite), and after that imported into a notebook with pandas.   

The tables can easily be joined via their keys, below an overview of features and keys: 

* Survey (PRIMARY KEY INT SurveyID, TEXT Description)
* Question (PRIMARY KEY QuestionID, TEXT QuestionText)
* Answer (PRIMARY KEY UserID, FOREIGN KEY SurveyID, FOREIGN KEY QuestionID, TEXT AnswerText)

With the data in the questionnaire , we will aim to get an idea of how much data was collected each year,
how the survey differed over the years, and how the sample of respondents differed over the years in terms of demographics. 

## Limitations

There is very limited information available about sampling decisions made for this questionnaire, thus we are not sure which 
types of analysis are suitable to run over the data collected with it. 

