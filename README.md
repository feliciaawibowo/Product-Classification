# Product-Classification

## Project Overview
This project focuses on text classification using machine learning techniques. The dataset consists of labeled text data and aims to predict categories based on the text content. Two main vectorization methods (TF-IDF and CountVectorizer) were used for feature extraction, and models (SVM and Random Forest) were trained and evaluated with both default and hyperparameter-tuned configurations.

## Dataset
Original Data: 12,606 rows
After Removing Duplicates: 10,454 rows

Features:
text: Input text data
label: Corresponding class labels

Data Split:
Training Set: 80%
Testing Set: 20%

## Model Architecture
### 1. Text Processing
Remove hashtags, numbers, and punctuation
Convert text to lowercase
Tokenize, remove stopwords, and apply stemming using the Porter Stemmer

### 2. Feature Extraction
**TF-IDF**: Converts text data to numerical vectors using term frequency-inverse document frequency
**CountVectorizer**: Converts text to numerical vectors based on term frequency

### 3. Models
**Support Vector Machine (SVM)**: Default and tuned hyperparameters
**Random Forest Classifier**: Default and tuned hyperparameters

## Training Details
### Hyperparameter Tuning
**SVM**: Grid search over C values (0.1, 1, 10) and kernels (linear, rbf).
**Random Forest**: Grid search over n_estimators (50, 100, 200), max_depth (10, 20, 30, None), and bootstrap (True, False).

## Evaluation Metrics
Accuracy: Proportion of correct predictions.
Precision: Proportion of true positives among predicted positives.
Recall: Proportion of true positives among actual positives.
F1 Score: Harmonic mean of precision and recall.

## Results


## Conclusion
The project demonstrates the effectiveness of text preprocessing and vectorization in text classification tasks. SVM with TF-IDF and tuned hyperparameters provided the best results, highlighting its robustness for this classification problem.
