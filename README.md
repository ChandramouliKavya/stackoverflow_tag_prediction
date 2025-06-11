# 🔖 Stack Overflow Automated Tag Prediction

## 📌 Problem Statement
Stack Overflow is one of the largest Q&A platforms for developers, where users post technical questions across a wide variety of programming domains. To improve the discoverability and organization of content, each question is assigned descriptive tags (e.g., python, web-development, machine-learning).

However, many users may find it difficult to assign the most appropriate tags, leading to inconsistencies and poor search experiences. This project aims to build a machine learning model that automatically predicts relevant tags based on a question’s title and body, enhancing searchability and reducing manual intervention.

## 🚀 Live Demo
### 🎯 Try the deployed web app here:
👉 https://huggingface.co/spaces/kavyasri0821/stack_overflow_tags

## 🕸️ Data Collection (Web Scraping)
Unlike using open datasets, this project uses custom web scraping to collect Stack Overflow data.

or Data can be collected from:
Stack Overflow public datasets available on platforms like Kaggle : https://www.kaggle.com/datasets/imoore/60k-stack-overflow-questions-with-quality-rate  or via the Stack Exchange API.

## 🔧 Tools Used:
BeautifulSoup

Requests

Selenium (if needed for dynamic content)

Python libraries for HTML parsing and cleaning

Extracted Fields:
Title: Short summary of the question

Body: Detailed description/content of the question

Tags: Actual tags associated with the question

The scraped data was stored in structured format (e.g., CSV/JSON) for further processing.

🧹 Data Preprocessing
To make the scraped textual data usable for machine learning, extensive cleaning was done:

Removed:

HTML tags

Code blocks

Special characters

Performed:

Lowercasing

Stopword removal

Tokenization

Lemmatization

## 🧠 Feature Extraction
To convert text into numerical format for ML models:

TF-IDF Vectorizer: Highlights important terms in a document

(Optional for future work) Word Embeddings: Word2Vec, FastText, BERT

## 🏷️ Problem Type
This is a Multi-label Classification problem:

A single question can belong to multiple tags.

The goal is to predict a set of relevant tags for a new question.

## 🧪 Feature Engineering
Tried multiple text vectorization methods:

Count Vectorizer

TF-IDF

(Planned) Word Embeddings

Extracted features from both title and body for richer input.




