# Amazon-Reviews-Sentiment-Analysis
Sentiment Analysis of Amazon Product Reviews using Machine Learning and NLP

This project focuses on sentiment analysis of Amazon product reviews using machine learning and natural language processing (NLP) techniques. The goal is to develop a Streamlit app capable of analyzing sentiments across various scenarios, including single-line reviews, multiple reviews from CSV files, and product reviews scraped from Amazon URLs.

Table of Contents

Overview
Dataset Used
Project Structure
Setup
Usage
Screenshots
Acknowledgements
Connect with Me
License
Overview

This project leverages machine learning models to perform sentiment analysis on Amazon product reviews. It includes support for:
Single-line review analysis
Multiple review analysis from CSV files
Product review analysis directly from Amazon URLs
The Streamlit app provides an interactive interface for users to explore sentiment analysis results.
Dataset Used

The Amazon reviews full score dataset is used, consisting of:
Training Set: 3,000,000 samples (600,000 samples for each review score from 1 to 5)
Testing Set: 650,000 samples (130,000 samples for each score)
Dataset link on Kaggle: Amazon Review Dataset
Project Structure

Amazon-Reviews-Sentiment-Analysis/
├── notebooks/                   # Jupyter notebooks for EDA and model development
├── test_files/                  # Test files to test sentiment analysis for multiple reviews
├── .streamlit/                  # Configuration files for the Streamlit app theme
├── models.p                     # Serialized models for sentiment analysis
├── review_analyzer.py           # Streamlit app code for interactive sentiment analysis
├── reviewscrapper.py            # Script for scraping Amazon reviews from URLs
├── requirements.txt             # Project dependencies for reproducibility
└── README.md                    # Project documentation
Setup

To get started, follow these instructions:

Navigate to the project directory:
cd Amazon-Reviews-Sentiment-Analysis
Install dependencies:
pip install -r requirements.txt
Run the Streamlit app:
streamlit run review_analyzer.py
Usage

Data Analysis and Model Development:
Explore the Jupyter notebook B8_Amazon.ipynb in the notebooks/ folder for in-depth data analysis and model training.
Web Scraping:
Use the reviewscrapper.py script to scrape product reviews from Amazon URLs.
python reviewscrapper.py --url "<Amazon Product URL>"
Interactive Sentiment Analysis:
Launch the Streamlit app to analyze single reviews, multiple reviews from CSV files, or reviews from Amazon URLs:
streamlit run review_analyzer.py
Screenshots

Streamlit App Interface
A user-friendly interface for running sentiment analysis.
Single Review Analysis
Upload or enter a single-line review for instant sentiment analysis.
Multi Review Analysis
Analyze multiple reviews from a CSV file for batch sentiment analysis.
Product URL Review Analysis
Input an Amazon product URL, and the app scrapes reviews and analyzes their sentiment.
Acknowledgements

This project was inspired by the following resources:
Introduction to Sentiment Analysis Techniques
NLP and Text Classification with Scikit-Learn

