# Smart News Analyzer

## Overview
Smart News Analyzer is an end-to-end NLP application that cleans and tokenizes news articles, benchmarks multiple classification models, and generates concise headlines—all wrapped in a real-time Streamlit dashboard. Leveraging spaCy, GloVe embeddings, BiLSTM, CNN, BERT, and the PEGASUS-xsum transformer, this project demonstrates full-cycle news analysis and generation workflows.

## Features
- **Data Processing**  
  - HTML and punctuation removal  
  - spaCy-based tokenization and lemmatization  
  - Sequence padding and train–validation splitting  

- **Modeling & Evaluation**  
  - CNN and BiLSTM classifiers with pretrained GloVe embeddings  
  - Fine-tuned BERT for advanced text classification  
  - Comparative performance tracking via classification reports and confusion matrices  

- **Headline Generation**  
  - Transformer-powered summary using PEGASUS-xsum  
  - Quality checks for generated headlines  

- **Interactive Dashboard**  
  - Real-time news classification and headline generation  
  - Model selection controls  
  - Performance visualization (accuracy metrics, confusion matrices)  
  - Input/output widgets for user-provided text  
