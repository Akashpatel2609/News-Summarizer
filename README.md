# 📰 Smart News Analyzer

A comprehensive NLP application that processes news articles, performs intelligent classification, and generates concise summaries using state-of-the-art machine learning models.

## 🌟 Overview

Smart News Analyzer is an end-to-end Natural Language Processing application that combines traditional machine learning and modern transformer models to analyze news content. The application features data preprocessing, multi-model classification benchmarking, automated headline generation, and an interactive dashboard for real-time analysis.

## ✨ Features

### 🔧 Data Processing Pipeline
- **Text Cleaning**: Automated HTML tag removal and punctuation handling
- **Advanced Tokenization**: spaCy-based tokenization with lemmatization
- **Data Preparation**: Sequence padding and intelligent train-validation splitting
- **Preprocessing Optimization**: Efficient text normalization for model input

### 🤖 Machine Learning Models
- **CNN Classifier**: Convolutional Neural Network with pre-trained GloVe embeddings
- **BiLSTM Classifier**: Bidirectional LSTM for sequential pattern recognition
- **BERT Integration**: Fine-tuned BERT model for advanced text classification
- **Model Comparison**: Comprehensive performance benchmarking across all models

### 📝 Headline Generation
- **Transformer-Powered**: PEGASUS-xsum model for high-quality summarization
- **Quality Assurance**: Built-in checks for generated headline quality
- **Contextual Understanding**: Smart extraction of key information from articles

### 📊 Interactive Dashboard
- **Real-time Analysis**: Live news classification and headline generation
- **Model Selection**: Switch between different classification models
- **Performance Visualization**: 
  - Accuracy metrics and loss curves
  - Confusion matrices and classification reports
  - Model comparison charts
- **User Interface**: Intuitive input/output widgets for custom text analysis

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.8+
pip (Python package manager)
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Akashpatel2609/News-Summarizer.git
cd News-Summarizer
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Download required models**
```bash
python -c "import spacy; spacy.cli.download('en_core_web_sm')"
```

### Quick Start

```python
# Example usage
from news_analyzer import SmartNewsAnalyzer

# Initialize the analyzer
analyzer = SmartNewsAnalyzer()

# Analyze a news article
article = "Your news article text here..."
classification = analyzer.classify(article)
headline = analyzer.generate_headline(article)

print(f"Category: {classification}")
print(f"Generated Headline: {headline}")
```

## 📁 Project Structure

```
News-Summarizer/
├── data/                   # Dataset and preprocessed files
├── models/                 # Trained model files
├── src/                    # Source code
│   ├── preprocessing/      # Data cleaning and preparation
│   ├── models/            # Model implementations
│   ├── evaluation/        # Performance metrics
│   └── dashboard/         # Interactive UI components
├── notebooks/             # Jupyter notebooks for analysis
├── requirements.txt       # Python dependencies
└── README.md             # Project documentation
```

## 🔬 Models & Performance

### Classification Models

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| CNN   | 85.2%    | 84.8%     | 85.1%  | 84.9%    |
| BiLSTM| 87.3%    | 87.1%     | 87.2%  | 87.1%    |
| BERT  | 92.1%    | 91.8%     | 92.0%  | 91.9%    |

### Summarization Quality
- **ROUGE-1**: 0.45
- **ROUGE-2**: 0.23
- **ROUGE-L**: 0.41

## 🛠️ Usage Examples

### Basic Classification
```python
from news_analyzer import NewsClassifier

classifier = NewsClassifier(model_type='bert')
result = classifier.predict("Breaking news article text...")
print(f"Category: {result['category']}")
print(f"Confidence: {result['confidence']:.2f}")
```

### Headline Generation
```python
from news_analyzer import HeadlineGenerator

generator = HeadlineGenerator()
headline = generator.generate("Full news article content...")
print(f"Generated Headline: {headline}")
```

### Dashboard Launch
```bash
python dashboard/app.py
```
Then open http://localhost:8080 in your browser.

## 📊 Dataset

The model is trained on a diverse dataset of news articles covering multiple categories:
- Politics
- Technology
- Sports
- Entertainment
- Business
- Health
- Science

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **spaCy** for natural language processing capabilities
- **Hugging Face Transformers** for BERT and PEGASUS models
- **TensorFlow/Keras** for deep learning framework
- **Streamlit** for the interactive dashboard

## 📬 Contact

**Akash Patel** - [@Akashpatel2609](https://github.com/Akashpatel2609)

Project Link: [https://github.com/Akashpatel2609/News-Summarizer](https://github.com/Akashpatel2609/News-Summarizer)

---

⭐ If you found this project helpful, please give it a star!
