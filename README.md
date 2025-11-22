# 🎬 Movie Review Sentiment Analysis with DVC

A complete machine learning pipeline for training and evaluating a sentiment classification model on movie reviews.  
This project demonstrates **DVC for data versioning, pipeline reproducibility, and experiment tracking**.

---

## 📋 Overview

This pipeline:

- Downloads movie review data from public sources  
- Preprocesses text (cleaning, tokenization, train/test split)  
- Trains a sentiment classifier using **TF-IDF + Logistic Regression**  
- Evaluates performance on a test set  
- Tracks all stages using **DVC**, ensuring reproducible ML workflows  

---

## 🏗️ Project Structure


movie-sentiment-dvc/
├── data/
│ ├── raw/ # Raw downloaded reviews (DVC-tracked)
│ └── processed/ # Train/test splits (DVC-tracked)
├── models/ # Trained model pickle files (DVC-tracked)
├── metrics/ # Evaluation metrics JSON
├── src/
│ ├── download_data.py # Download and prepare raw data
│ ├── preprocess.py # Clean and split data
│ ├── train.py # Train the classifier
│ └── evaluate.py # Evaluate performance
├── dvc.yaml # Pipeline definition
├── params.yaml # Hyperparameters
├── requirements.txt # Dependencies
└── README.md


