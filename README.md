# A-Comprehensive-Sentiment-Analysis-Framework-on-Twitter-Data

Authors: Swayamprava Aich, Radhika Kumavat, Divya Naika, Aman Phogat, Deep Patel

Course: APLN-552: Special Topics in Natural Language Processing

Institution: Montclair State University

## Abstract:

Twitter generates vast amounts of data reflecting public sentiment. This project uses supervised machine learning to analyze sentiments in tweets. We preprocess the tweets by removing special characters, stopwords, and performing lemmatization. We then apply TF-IDF vectorization to transform the preprocessed tweets into a numerical format, capturing the importance of words in each tweet relative to the entire dataset.
To improve prediction accuracy, we employ an ensemble of classifiers, including Random Forest, Support Vector Machine, Logistic Regression, and Multinomial Naive Bayes. Each classifier provides a unique perspective on the sentiment analysis task, and by combining their predictions, we achieve a more robust and accurate sentiment classification model.
Our results demonstrate the efficacy of combining machine learning techniques for sentiment analysis on Twitter data. The ensemble model consistently outperforms individual classifiers, showcasing the benefit of leveraging diverse algorithms to capture different aspects of sentiment in tweets. This approach holds promise for understanding public opinion and sentiment trends on social media platforms.

## Introducation:

Twitter provides a rich source of data for sentiment analysis. This report explores Twitter-based Sentiment Analysis (TSA) using supervised machine learning classifiers. We discuss the significance of TSA in commercial and socio-political contexts and outline the processes involved in collecting, preprocessing, and classifying Twitter data.

## Dataset:
The dataset that was used was obtained from “Kaggle” (https://www.kaggle.com/datasets/kazanova/sentiment140) dataset. The dataset snpashot has been attached below for reference -
![image](https://github.com/AichSwayamprava/A-Comprehensive-Sentiment-Analysis-Framework-on-Twitter-Data/assets/128501002/e7144ea9-4c76-4aa0-896d-3daf2c4468fa)

It contains 1,600,000 tweets extracted using the twitter API. The tweets have been annotated (0 = negative, 2 = neutral, 4 = positive) and they can be used to detect sentiment. But only 40000 rows where randomly selected from this dataset, with equal distribution of positive and negative tweets, i.e. neutral tweets were ignored as this study focuses on binary classification.

## Data Description:

Dataset Composition: The dataset includes fields such as 'target' (indicating sentiment polarity), 'ids', 'date', 'flag', 'user', and 'text'. We preprocess the data to create a balanced subset with 20,000 tweets each for negative, neutral, and positive sentiments.

Data Processing and Balancing: We use the VADER tool to reclassify and balance the dataset, ensuring uniform representation across sentiment classes.

Data Cleaning and Preprocessing: We perform data cleaning to remove irrelevant and noisy components from the text data, including URLs, HTML tags, special characters, and user mentions. We also perform tokenization, stop word removal, lemmatization, and expansion of contractions.

## TF-IDF Vectorization for Feature Extraction
We use TF-IDF vectorization to transform preprocessed text into a numerical format suitable for machine learning algorithms. TF-IDF helps in selecting and weighting words based on their importance in the document and the corpus.

## Models and Methods Employed in Sentiment Analysis
We employ several machine learning models, including Logistic Regression, Naive Bayes, SVM, Decision Trees, and an Ensemble Method (Voting Classifier), to perform sentiment analysis on the textual data. Each model offers unique advantages and is chosen based on its suitability for the task.

## Experiments & Observations
We evaluate the performance of the sentiment analysis models using metrics such as accuracy, precision, recall, and F1-score. SVM and the Voting Classifier show superior performance, demonstrating the effectiveness of ensemble methods.

## Conclusions & Roadmap
We conclude that traditional machine learning models are effective for sentiment analysis in textual data contexts. Future work could involve integrating deep learning techniques, exploring advanced features, and incorporating more diverse datasets to further improve model performance.


