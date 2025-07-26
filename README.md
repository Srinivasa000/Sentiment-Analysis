# Sentiment Analysis on Movie Reviews

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-Scikit--learn%20%7C%20NLTK-orange.svg)

A comprehensive Python project to perform sentiment analysis on text data. This implementation includes two approaches:
1.  **Document-Level Analysis:** Classifies an entire movie review as 'positive' or 'negative' using a classic machine learning pipeline (TF-IDF + Logistic Regression).
2.  **Sentence-Level Analysis:** Analyzes the tone of each individual sentence in a review using the VADER sentiment lexicon to capture nuanced opinions.

## Features
-   **Text Preprocessing:** Cleans and normalizes raw text for better model performance.
-   **Machine Learning Model:** Uses `scikit-learn` to build a robust classification pipeline.
-   **Granular Analysis:** Employs NLTK's VADER to get positive, negative, and neutral scores for each sentence.
-   **Easy to Use:** Scripts are ready to run with sample data included.

## Tech Stack
-   **Language:** Python 3.9+
-   **Core Libraries:**
    -   `scikit-learn`: For the machine learning pipeline (TF-IDF, Logistic Regression).
    -   `pandas`: For data manipulation.
    -   `nltk`: For text processing, sentence tokenization, and VADER analysis.

## Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/sentiment-analysis.git](https://github.com/your-username/sentiment-analysis.git)
    cd sentiment-analysis
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Your `requirements.txt` file should contain: `pandas`, `scikit-learn`, `nltk`)*

4.  **Download NLTK data:**
    Run this Python script once to download the necessary models.
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('vader_lexicon')
    ```

## Usage

The project contains two main scripts for demonstration.

#### 1. Document-Level Sentiment Analysis
This script trains a model on a sample dataset and predicts the sentiment of a new review.

**To run:**
```bash
python main_document_sentiment.py
