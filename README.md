# Sentiment Analysis Using Machine Learning

## Overview

This project focuses on classifying text into three sentiment categories: **Negative, Neutral, and Positive** using Natural Language Processing (NLP) and Machine Learning techniques.

The project explores text preprocessing methods, TF-IDF feature extraction, and Logistic Regression to build and evaluate a sentiment classification model.

## Objectives

- Perform text preprocessing and cleaning.
- Handle stopwords while preserving important negation words.
- Compare stemming and lemmatization techniques.
- Convert text into numerical features using TF-IDF.
- Train and evaluate Logistic Regression models.
- Investigate class imbalance using class-weight balancing.
- Test the trained model on custom text examples.

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Workflow

1. **Data Loading and Exploration**  
   Load the dataset and examine its structure, sentiment labels, and class distribution.

2. **Text Preprocessing**  
   Clean and normalize text, expand common contractions, tokenize text, remove punctuation and stopwords, and apply stemming or lemmatization.

3. **Feature Extraction**  
   Use TF-IDF Vectorization with unigram and bigram features to convert text into numerical representations.

4. **Model Training**  
   Train Logistic Regression models using the extracted text features.

5. **Model Comparison**  
   Compare stemming and lemmatization approaches and evaluate class-weight balancing to address differences in sentiment class distribution.

6. **Model Evaluation**  
   Evaluate the models using accuracy, precision, recall, F1-score, classification reports, and confusion matrices.

7. **Custom Predictions**  
   Test the trained model on new sentences and examine predicted sentiment labels and class probabilities.

## Model Performance

The following results were observed during model evaluation.

| Model | Accuracy | Macro F1-Score |
|---|---:|---:|
| Logistic Regression with Stemming | 68.89% | 0.6909 |
| Logistic Regression with Lemmatization | 68.43% | 0.6861 |
| Balanced Logistic Regression | 69.94% | 0.7033 |

The balanced Logistic Regression model achieved the best observed results among these experiments, with an accuracy of **69.94%** and a macro F1-score of **0.7033**.

*Note: These results reflect the recorded notebook outputs. Final results should be verified after rerunning the updated preprocessing and model evaluation cells.*

## Sentiment Labels

| Label | Sentiment |
|---:|---|
| -1 | Negative |
| 0 | Neutral |
| 1 | Positive |

## Example Predictions

| Input Text | Predicted Sentiment |
|---|---|
| This game is absolutely amazing, I love every minute of it! | Positive |
| The product is terrible and a complete waste of money. | Negative |
| The package arrived yesterday. | Negative |
| The graphics are beautiful, but the gameplay is boring. | Negative |
| I thought this movie would be bad, but it was surprisingly good. | Positive |

These examples illustrate the model's predictions. Neutral and mixed-sentiment examples require further evaluation and improvement.

## Key Learnings

- Understanding the importance of text preprocessing in NLP.
- Comparing stemming and lemmatization for text classification.
- Applying TF-IDF to represent textual data.
- Evaluating classification models beyond accuracy using macro F1-score.
- Exploring class weighting to improve performance across sentiment categories.
- Identifying misclassifications through custom predictions.

## Future Improvements

- Experiment with different machine learning algorithms.
- Improve neutral and mixed-sentiment classification.
- Preserve negation and contextual information more effectively.
- Perform hyperparameter tuning.
- Evaluate additional feature extraction techniques.
- Explore advanced NLP models such as transformer-based classifiers.

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone <your-repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd <your-project-folder>
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy nltk scikit-learn matplotlib seaborn jupyter
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open the sentiment analysis notebook and run the cells in order.

## Conclusion

This project demonstrates an end-to-end text classification workflow using NLP and machine learning. Comparing preprocessing methods and Logistic Regression configurations helped identify the best-performing model among the tested experiments. The results also highlight opportunities to improve neutral and context-dependent sentiment classification.
