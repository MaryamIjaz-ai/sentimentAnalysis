# sentimentAnalysis
sentiment analysis of internship feedback using logistic regression and BERT
📊 Sentiment Analysis of Internship Feedback
Task: Classify feedback as Positive or Negative using machine learning and deep learning models

📅 Date: July 2025
👤 Author: [Maryam Ijaz]

🎯 Objective
To analyze intern feedback and reviews to determine sentiment (positive or negative) using two different approaches:

Logistic Regression with TF-IDF – A classical machine learning baseline

BERT (Bidirectional Encoder Representations from Transformers) – A modern transformer-based language model

The ultimate goal is to identify areas of intern dissatisfaction and improve internship program quality.

📁 Dataset Description
Source: Intern feedback collected and labeled manually

Size: 30 entries (15 positive, 15 negative)

Columns:

feedback: The text of the intern’s review

sentiment: Label — "positive" or "negative"

label: Encoded — 1 for positive, 0 for negative

🧪 Model 1: Logistic Regression + TF-IDF
✅ Steps:
Preprocessing with TF-IDF (top 1000 features)

Class balancing via class_weight='balanced'

Stratified train-test split

Evaluated using confusion matrix and classification report

🤖 Model 2: BERT (Transformer-Based Classifier)
✅ Steps:
Used pre-trained bert-base-uncased from Hugging Face

Fine-tuned using Trainer API on labeled data

Handled padding/truncation and attention masks

No external logging (e.g., wandb)

📉 Results:
Metric	Positive	Negative
Precision	High	High
Recall	High	High
F1-Score	~0.90+	~0.85+
Accuracy	~90%+	

📌 Insights:
Better at understanding context (e.g., sarcasm, subtle tone)

Requires more compute, but significantly better performance

Generalizes well, even on small datasets

