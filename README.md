# A-Comprehensive-Sentiment-Analysis-Framework-on-Twitter-Data

Authors: Swayamprava Aich, Radhika Kumavat, Divya Naika, Aman Phogat, Deep Patel

Course: APLN-552: Special Topics in Natural Language Processing

Institution: Montclair State University

## Abstract:

Twitter, a prolific source of data, mirrors the public sentiment dynamically. This project uses supervised machine learning to decode sentiments embedded in tweets. We meticulously preprocess tweets by removing special characters and stopwords and performing lemmatization to cleanse the text data. Subsequently, TF-IDF vectorization is employed to convert the preprocessed tweets into a numerical format that emphasizes the significance of words within each tweet relative to the dataset.

To enhance the accuracy of sentiment predictions, we deploy an ensemble of classifiers—Support Vector Machine, Logistic Regression, Decision Tree, and Multinomial Naive Bayes. Each classifier contributes a distinct perspective to the sentiment analysis task, and their combined predictions yield a robust and precise sentiment classification model. Our approach is particularly tailored to handle bilingual tweets, adding a layer of complexity and relevance to the analysis given the diverse linguistic fabric of Twitter.

The results demonstrate the efficacy of the ensemble model over individual classifiers, underscoring the advantages of leveraging a diverse set of algorithms to capture various facets of sentiment in tweets. This methodological framework promises significant utility in gauging public opinion and tracking sentiment trends on social media platforms. Future work could explore real-time analysis and the integration of more complex linguistic features to further enhance the model’s accuracy and applicability.

## Introduction:

Twitter provides a rich source of data for sentiment analysis. This report explores Twitter-based Sentiment Analysis (TSA) using supervised machine learning classifiers. We discuss the significance of TSA in commercial and socio-political contexts and outline the processes involved in collecting, preprocessing, and classifying Twitter data.

## Dataset:
The dataset that was used was obtained from “Kaggle” (https://www.kaggle.com/datasets/kazanova/sentiment140) dataset. The dataset snapshot has been attached below for reference -
![image](https://github.com/AichSwayamprava/A-Comprehensive-Sentiment-Analysis-Framework-on-Twitter-Data/assets/128501002/e7144ea9-4c76-4aa0-896d-3daf2c4468fa)

It contains 1,600,000 tweets extracted using the twitter API. The tweets have been annotated (0 = negative, 2 = neutral, 4 = positive) and they can be used to detect sentiment. But only 60000 rows were randomly selected from this dataset, with equal distribution of positive, netural and negative tweets.

## Data Description:

Dataset Composition: The dataset includes fields such as 'target' (indicating sentiment polarity), 'ids', 'date', 'flag', 'user', and 'text'. We preprocess the data to create a balanced subset with 20,000 tweets each for negative, neutral, and positive sentiments.

Data Processing and Balancing: We use the VADER tool to reclassify and balance the dataset, ensuring uniform representation across sentiment classes.

Data Cleaning and Preprocessing: We perform data cleaning to remove irrelevant and noisy components from the text data, including URLs, HTML tags, special characters, and user mentions. We also perform tokenization, stop word removal, lemmatization, and expansion of contractions.

<img width="249" alt="image" src="https://github.com/AichSwayamprava/A-Comprehensive-Sentiment-Analysis-Framework-on-Twitter-Data/assets/128501002/376e6874-3ce9-4979-8957-56d2dfaacede">



## TF-IDF Vectorization for Feature Extraction
We use TF-IDF vectorization to transform preprocessed text into a numerical format suitable for machine learning algorithms. TF-IDF helps in selecting and weighting words based on their importance in the document and the corpus.

## Models and Methods Employed in Sentiment Analysis
We employ several machine learning models, including Logistic Regression, Naive Bayes, SVM, Decision Trees, and an Ensemble Method (Voting Classifier), to perform sentiment analysis on the textual data. Each model offers unique advantages and is chosen based on its suitability for the task.

## Experiments & Observations
We evaluate the performance of the sentiment analysis models using metrics such as accuracy, precision, recall, and F1-score. SVM and the Voting Classifier show superior performance, demonstrating the effectiveness of ensemble methods.

## Conclusions & Roadmap
We conclude that traditional machine learning models are effective for sentiment analysis in textual data contexts. Future work could involve integrating deep learning techniques, exploring advanced features, and incorporating more diverse datasets to further improve model performance.

## Reference Papers

1.	A.Pak and P. Paroubek. „Twitter as a Corpus for Sentiment Analysis and Opinion Mining". In Proceedings of the Seventh Conference on International Language Resources and Evaluation, 2010, pp.1320-1326
2.	R. Parikh and M. Movassate, “Sentiment Analysis of User- GeneratedTwitter Updates using Various Classification Techniques",CS224N Final Report, 2009
3.	Po-Wei Liang, Bi-Ru Dai, “Opinion Mining on Social MediaData", IEEE 14th International Conference on Mobile Data Management,Milan, Italy, June 3 - 6, 2013, pp 91-96, ISBN: 978-1-494673-6068-5, http://doi.ieeecomputersociety.org/10.1109/MDM.2013.
4.	Pablo Gamallo, Marcos Garcia, “Citius: A Naive-Bayes Strategyfor Sentiment Analysis on English Tweets", 8th InternationalWorkshop on Semantic Evaluation (SemEval 2014), Dublin, Ireland,Aug 23-24 2014, pp 171-175
5.	J. Kamps, M. Marx, R. J. Mokken, and M. De Rijke, “Using wordnet to measure semantic orientations of adjectives,” 2004.
6.	R. Xia, C. Zong, and S. Li, “Ensemble of feature sets and classification algorithms for sentiment classification,” Information Sciences: an International Journal, vol. 181, no. 6, pp. 1138–1152, 2011.
7.	ZhunchenLuo, Miles Osborne, TingWang, An effective approachto tweets opinion retrieval", Springer Journal onWorldWideWeb,Dec 2013, DOI: 10.1007/s11280-013- 0268-7.
8.	Li Rao,” Sentiment Analysis of English Text with Multilevel Features”, January  2022
9.	Go, R. Bhayani, L.Huang. “Twitter Sentiment ClassificationUsing Distant Supervision". Stanford University, Technical Paper,2009
10.	Bollegala, D., Weir, D., & Carroll, J.. Cross-Domain SentimentClassification using a Sentiment Sensitive Thesaurus. Knowledge andData Engineering, IEEE Transactions on, 25(8), 1719-1731,2013
11.	Agarwal, B. Xie, I. Vovsha, O. Rambow, R. Passonneau, “Sentiment Analysis of Twitter Data", In Proceedings of the ACL 2011Workshop on Languages in Social Media,2011 , pp. 30-38
12.	 L. Barbosa, J. Feng. “Robust Sentiment Detection on Twitterfrom Biased and Noisy Data". COLING 2010: Poster Volume,pp. 36-44.


