# NLP **Sentiment Analysis User Reviews** (in progress Dec 2024)
***The project is currently in development, right now on stage 2: preprocessing, with tasks being approached iteratively for efficient analysis and model development.***

This project aims to perform a sentiment analysis on a dataset of Amazon product reviews to classify sentiments as positive or negative based on ratings (1-5 stars).


## **1. Stage: DATA - EDA**

📈Data Exploration: Analyzed review distributions, polarity, and subjectivity. Visualized the frequency of terms, top bigrams/trigrams, and created word clouds for deeper insights.

💻Text Preprocessing: Cleaned and preprocessed textual data by removing noise, stop words, and special characters. Applied tokenization, lemmatization, and handled outliers.

⬅️TF-IDF Analysis: Extracted the top important words using TF-IDF, identifying key terms relevant to sentiment classification.

⌨️Word Embeddings: Trained Word2Vec to capture word relationships, visualized the most similar words for key terms.


## **Overall data Exploration:**

**Sentiment Distribution:**
The reviews are well-balanced, with a mix of positive, negative, and neutral sentiments. The model can be effectively trained using a binary sentiment classification (positive vs negative).

**Textual Insights:**
Common terms in both positive and negative reviews were identified, with "good", "work", "use", and "product" frequently appearing. These terms help capture the sentiment associated with product functionality and user experience.

**Polarity and Subjectivity:** 
The dataset contains a mix of subjective and objective reviews, with polarity values indicating a predominance of neutral to slightly positive sentiment. This suggests the need for techniques that handle both sentiment and opinion aspects.

**Preprocessing Readiness:** 
I performed essential cleaning steps, such as removing stopwords and non-alphabetic characters, and tokenization, ensuring the data is ready for modeling. However, deeper preprocessing will be handled in the next phase to optimize for machine learning.

**TF-IDF and Word2Vec Insights:** 
The analysis of word importance and embeddings revealed the most relevant words for sentiment classification, with the ability to identify similar words based on their context.


