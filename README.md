**Sentiment Analysis on Amazon Reviews (NLTK + Python)**.
This project demonstrates how to perform sentiment analysis on Amazon product reviews using Natural Language Toolkit (NLTK) and scikit-learn.

**Features**.
Loads Amazon review dataset (20,000+ samples)
Preprocesses text using:
Tokenization
Stopword removal
Lemmatization
Applies the preprocessing pipeline to clean review text
Trains and evaluates sentiment classification model

**Dataset**.
Amazon reviews dataset is loaded from PyCaret’s GitHub.

It contains:
reviewText: customer review
Positive: sentiment label (1 = positive, 0 = negative)

**🛠️ Preprocessing Steps**.

Tokenization – split reviews into words
Stopword Removal – remove common English words (e.g., the, and, is)
Lemmatization – reduce words to base form (running → run)
Rejoin Tokens – convert processed tokens back into a string

**📊 Model Evaluation**.
Confusion Matrix
[[ 1131  3636]
 [  576 14657]]

**Classification Report**.
Class	Precision	Recall	F1-Score	Support
0 (Negative)	0.66	0.24	0.35	4767
1 (Positive)	0.80	0.96	0.87	15233

**Overall Accuracy: 79%**.
Model performs well on positive reviews, but struggles with recall for negative reviews.

✅ This project builds a full pipeline from text preprocessing → feature extraction → sentiment classification → evaluation, and can be extended with advanced ML/DL models for better performance.
