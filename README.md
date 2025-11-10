# Multilingual Language Identification Model

This project builds a language identification classifier for five languages: Swahili, English, Spanish, Hindi, and Aragonese. It uses TF-IDF character n-grams and a tuned Naive Bayes model to predict the language of a given text.

## Features
- Supports five languages: Swahili (sw), English (en), Spanish (es), Hindi (hi), and Aragonese (an)
- Uses character-level TF-IDF (1–5 n-grams) for multilingual representation
- Includes data cleaning, Unicode normalization, and class balancing
- Hyperparameter tuning using GridSearchCV
- Evaluation metrics include accuracy, classification report, and confusion matrix
- Tests model on unseen text for generalization

## Workflow
1. Load datasets from Hugging Face:
   - wikitext (English)
   - swahili_news (Swahili)
   - cfilt/iitb-english-hindi (Hindi)
   - projecte-aina/ES-AN_Parallel_Corpus (Spanish & Aragonese)
2. Clean and normalize text data
3. Balance dataset across all languages
4. Vectorize text using TF-IDF character n-grams
5. Train Multinomial Naive Bayes with GridSearchCV tuning
6. Evaluate model on validation and test data
7. Predict unseen sentences and display confidence scores

