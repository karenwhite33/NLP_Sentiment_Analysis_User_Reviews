# NLP **Sentiment Analysis User Reviews**

Drive link to full folders: https://drive.google.com/drive/folders/1BSvsK9gnz1m4nSbdmZfbohlbCA0HceyO?usp=sharing

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

__________________________________

## **2. Stage: DATA PRE-PROCESSING**

**💻Data Cleaning and Transformation:**

Removed HTML, retaining only meaningful text.
Converted numeric values to words for better NLP understanding.
Stripped non-alphanumeric characters for relevant content.
Standardized text to lowercase for consistency.

**🛑Stopwords Removal:**

Applied language-specific stopword removal using dynamic detection (English, Spanish, etc.).
Implemented custom tokenization to ensure accuracy without relying on external tools.


**📖Lemmatization:**

Utilized WordNet lemmatizer to reduce words to their base form, improving semantic consistency.


**💬Text Preprocessing Pipeline:**

Automated preprocessing in a single Python function for consistency and reproducibility.
Optimized pipeline for speed and memory usage, handling large datasets efficiently.


## **Overall data Pre-processing:**

**Positive Reviews:**

Common terms like "good", "great", "love", "quality", and "perfect" dominate, indicating high customer satisfaction and product endorsement.
"Recommend" strongly suggests positive sentiment and willingness to promote the product.

**Negative Reviews:**

Words like "dont", "poor", "waste", "returned", and "cheap" reveal significant dissatisfaction and product issues.
Frequent mentions of "returned" signal problems leading to product returns.

**Frequent vs. Specific Terms:**

High-frequency words like "good" and "love" reflect general satisfaction.
Low-frequency terms (e.g., "waste", "returned") pinpoint specific issues such as product defects or poor quality.

**Effective Preprocessing:**

Stopword removal and lemmatization streamlined text, making sentiment analysis more accurate.
Tokenization improved the granularity of analysis, focusing on meaningful words that represent key product feedback.

**Data Cleaning Impact:**

Noise reduction via text cleaning and stopword removal enhanced the focus on key sentiment-driving words, enabling better feature extraction for sentiment modeling.

## 💡**Plan for stage 3:**

Leverage advanced NLP models (e.g., TF-IDF, word embeddings) to capture deeper context and improve sentiment classification. Creat and train 2 ML models to compare performances.

## 💡**Plan for stage 4:**
Create a Deep Learning model from one simple layer to iterate over more models to find better hiperparameters and performance.
