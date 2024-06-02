# Financial Document Classifier
This repository contains a machine learning solution for classifying tables from financial statements into several categories, including Income Statements, Balance Sheets, Cash Flows, Notes, and Others. The solution is designed to handle structured and semi-structured data in HTML and PDF formats.
Features

## Data Ingestion: 
Load and convert HTML files to PDF format for data exploration and quality purposes.
## Data Extraction: 
Extract text data from PDF files or parse it directly from HTML documents.
## Data Preprocessing: 
Preprocess the extracted text by converting it to lowercase, removing special characters, stop words, and whitespaces. Normalize and tokenize the text data.
## Feature Engineering: 
Create a DataFrame with labels, extracted text, and identifiers (maximum occurring five terms in each document type for classification purposes).
## Data Balancing: 
Apply oversampling methods to preprocess the data and address imbalance, if present.
## Feature Vectorization: 
Convert text data to numerical form using TF-IDF vectorization.
## Model Training: 
Train three separate machine learning models using Random Forests, Naive Bayes, and XGBoost algorithms.
## Model Persistence: 
Save the trained models for future use.
## Model Testing: 
Extract and preprocess data from a sample file, vectorize the text data, and pass it through the trained models for prediction.

# Getting Started
Clone the repository:

Copy codegit clone https://github.com/PrerArya/financial-document-classifier.git

Prepare your data in HTML or PDF format.
1.Update the data ingestion and preprocessing steps according to your data format and requirements.
2.Train the models using the provided algorithms or introduce new algorithms as needed.
3.Evaluate the model performance using appropriate metrics.
4.Use the trained models to classify new documents.

# Performance
The trained models achieved the following accuracies on the given problem:

## Random Forest: 98% accuracy
## Naive Bayes: 91% accuracy
## XGBoost: 98% accuracy

The Random Forest and XGBoost algorithms performed exceptionally well, achieving a 98% accuracy rate.

# Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
License
