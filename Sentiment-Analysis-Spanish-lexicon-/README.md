# Sentiment Analysis on Spanish Movie Reviews

[Full project version here](https://ygs1629.github.io/Sentiment-Analysis-Spanish-lexicon-/)

## Overview
This project performs **sentiment analysis** on Spanish movie reviews using both **lexicon-based approaches** and **supervised machine learning models**.  
It explores the relationship between textual sentiment expressed in reviews and numerical movie ratings, analyzing how sentiment varies across different film genres.  
The project combines **natural language processing (NLP)** techniques with **statistical analysis** to extract meaningful insights from unstructured text data.

---

## Objective
The primary goal is to apply **opinion mining techniques in Spanish** to analyze movie reviews, examining the relationship between review polarity and factors such as:
- Film genre  
- Average movie rating  

The project compares **lexicon-based methods** with **supervised learning approaches** (Naïve Bayes and Logistic Regression) to determine the most effective classification strategy for **Spanish sentiment analysis**.

---

##  Data
The dataset was originally shared in an **academic context** by a university professor.  
Due to **privacy and intellectual property restrictions**, the full dataset and its source cannot be disclosed.  

For this project, I worked with a **stratified 20% sample by film genre**, ensuring representativeness across categories while preserving confidentiality.  

The dataset consists of the following variables:
- **Review text content**  
- **Movie titles and genres**  
- **Individual review titles**  
- **Average film ratings**  
- **Gender classification of films**  

From this data, I extracted **sentiment polarity** at both:
- The **individual review level**  
- The **movie aggregate level**  

This repository therefore focuses on the **analytical workflow, machine learning models, and insights**, which are transferable to other real-world datasets.

---

## Techniques

- **Text Preprocessing**: Tokenization, lowercase conversion, punctuation removal, stopword elimination  
- **Lexicon-Based Analysis**: NRC sentiment dictionary for Spanish with positive/negative classification  
- **Feature Engineering**: Term-Document Matrix creation with dimensionality reduction  
- **Supervised Models**: Naïve Bayes and Logistic Regression   
- **Visualization**: Word clouds, correlation plots and sentiment distribution histograms  

---

## Evaluation Metrics
Models were evaluated using:
- **Accuracy** → Overall classification correctness  
- **F1-score** → Harmonic mean of precision and recall  
- **Kappa** → Agreement coefficient correcting for random chance  

---

## Major Findings
-**Weak Correlation**: A weak negative linear relationship (-0.28) was found between sentiment polarity and numerical ratings

-**Genre Dependencies**: Sentiment distribution varies significantly by genre, with Drama showing substantial negative reviews linked to its thematic nature rather than quality

-**Model Performance**: Naïve Bayes achieved superior performance (89.7% accuracy, Kappa = 0.784) compared to Logistic Regression (89.4% accuracy, Kappa = 0.773)

-**Lexicon Limitations**: Dictionary-based approach performed marginally better than random (56.1% accuracy, Kappa = 0.064) but remained inadequate for reliable classification

-**Qualitative Insights***: Word clouds revealed distinct vocabulary patterns between positive and negative reviews, with negative feedback focusing on narrative flaws while positive reviews emphasized technical aspects and humor

---

## Some Key Visual Takeaways 
### Models evaluation metrics
![Model evaluation metrics comparison](https://github.com/ygs1629/Sentiment-Analysis-Spanish-lexicon-/blob/main/images/Comparaci%C3%B3n%20de%20m%C3%A9tricas%20por%20enfoque%20de%20clasificaci%C3%B3n.jpeg)

### Polarization histogram:
![Histogram of polarization](https://github.com/ygs1629/Sentiment-Analysis-Spanish-lexicon-/blob/main/images/Distribuci%C3%B3n%20de%20polaridad%20por%20g%C3%A9nero%20cinematogr%C3%A1fico.jpeg)
---

## Skills and Tools
- **Programming**: R  
- **Libraries**: tidyverse, tidytext, tm, syuzhet, caret, glmnet, wordcloud, ggplot2  
- **NLP Techniques**: Tokenization, sentiment analysis, term-document matrices  
- **Machine Learning**: Naïve Bayes, Logistic Regression, model evaluation  
- **Data Visualization**: Histograms, scatter plots, word clouds, comparative metrics charts  
- **Data Processing**: Text cleaning, feature engineering, correlation analysis  

---
**Note**: HTML in Spanish; description here is in English for international visibility and portfolio presentation. The graphics shown are all own-elaborated.This educational project extends a university assignment. The NLP techniques (learned at the university degree) and insights gained are broadly transferable to other text-based data applications.

