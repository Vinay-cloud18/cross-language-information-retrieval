# 🚀 Cross-Language Information Retrieval (CLIR)

> A research-oriented implementation of a German → English Cross-Language Information Retrieval system integrating Statistical Machine Translation and Okapi BM25 ranking.

---

## 🌍 Overview

This project implements a **Cross-Language Information Retrieval (CLIR)** system capable of:

- Translating German queries into English
- Retrieving relevant English documents
- Ranking documents using **Okapi BM25**
- Evaluating retrieval performance using **Mean Average Precision (MAP)**

The system integrates **Information Retrieval, Language Modeling, and Statistical Machine Translation** into a unified pipeline.

---

## 🧠 System Architecture

German Query
↓
Translation Model (IBM Model 1)
↓
Noisy Channel Model
↓
English Query
↓
BM25 Ranking Engine
↓
Ranked English Documents
↓
Evaluation (MAP)


---

## 🔎 Core Components

### 📌 1. Information Retrieval Engine
- Inverted Index Construction
- TF-IDF Term Weighting
- Okapi BM25 Ranking Model
- Document Length Normalization

### 📌 2. Language Modeling
- Unigram Model (Add-k / Laplace Smoothing)
- Trigram Model (Katz Backoff Smoothing)
- Perplexity Evaluation

### 📌 3. Translation Model
- IBM Model 1 (Expectation Maximization Algorithm)
- Word Alignment (Bidirectional Intersection)
- Translation Probability Tables
- Noisy Channel Decoding

### 📌 4. Evaluation Metrics
- Perplexity (Language Model Quality)
- Mean Average Precision (Retrieval Quality)

---

## 📊 Experimental Results

| Model | Perplexity |
|--------|------------|
| Unigram (Best k) | ~613 |
| Trigram (Katz Backoff) | ~461 |

Trigram modeling significantly improved sentence prediction quality.

MAP improved when using **Noisy Channel translation** compared to direct word translation.

---

## 🛠 Technologies Used

- Python
- NLTK
- IBM Model 1
- Okapi BM25
- TF-IDF
- Statistical NLP Techniques

---

## 📁 Dataset

- Europarl Parallel Corpus (German-English)
- Wikipedia English document corpus
- German query set with relevance judgments

---

## ⚡ Key Learnings

- Effect of smoothing techniques in statistical language models
- Importance of evaluation metrics in IR systems
- Limitations of word-based translation approaches
- Trade-offs between translation quality and retrieval performance

---

## 🚀 Future Improvements

- Phrase-based statistical translation
- Neural Machine Translation (NMT)
- Cross-lingual embeddings
- Transformer-based multilingual retrieval

---

## 👨‍💻 Author

**G Yuva Sai Vinay**  
Computer Science AI and DS Undergraduate  
Interested in Systems, NLP, and Research-driven Computing

---
