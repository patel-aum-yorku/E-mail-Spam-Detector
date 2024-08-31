# E-mail-Spam-Detector

## Project Overview

This project is an implementation of a spam classifier using Naive Bayes, a probabilistic machine learning model based on Bayes' Theorem. The classifier is designed to identify and filter out spam messages from legitimate messages in an SMS dataset.

## Dataset

The project uses the SMS Spam Collection dataset, which consists of 5,574 SMS messages. Each message is labeled as either "ham" (legitimate) or "spam." The dataset contains one message per line, with the label in the first column and the raw text of the message in the second column.

## Naive Bayes Classification

### Intuition

Naive Bayes is a simple yet effective classification technique. It works by calculating the posterior probability for each class label (ham or spam) based on the features extracted from the SMS messages. The model assumes that the presence of a particular feature in a class is independent of the presence of any other feature, hence the term "naive."

### Steps Involved

1. **Prior Probability**: The prior probability of each class is calculated based on the frequency of each class in the dataset.
2. **Likelihood**: The likelihood of the features given each class is computed.
3. **Posterior Probability**: The posterior probability is determined by combining the prior probability with the likelihood using Bayes' Theorem.

### Mathematical Foundation

The mathematical formula used in Naive Bayes classification is:

\[ P(Y|X) = \frac{P(X|Y) \cdot P(Y)}{P(X)} \]

Where:
- \( P(Y|X) \) is the posterior probability of class \( Y \) given the features \( X \).
- \( P(X|Y) \) is the likelihood of features \( X \) given class \( Y \).
- \( P(Y) \) is the prior probability of class \( Y \).
- \( P(X) \) is the marginal likelihood of features \( X \).

## Implementation

The project is implemented using Python, with the following main components:
- **Data Preprocessing**: The SMS data is cleaned and tokenized to prepare it for the Naive Bayes classifier.
- **Feature Extraction**: Features are extracted from the SMS messages, such as word frequencies.
- **Model Training**: The Naive Bayes model is trained on a portion of the dataset.
- **Model Evaluation**: The model is evaluated on a test set to determine its accuracy in classifying messages as ham or spam.

## Usage

To run the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/E-mail-Spam-Detector.git
2. Download all the dependencies, it is preferred to use Anaconda but if you want to ue any other editor then
   ```bash
   pip install required-dependecies

`required-dependencies` -  look into notebook and install all the packages that are being imported.
