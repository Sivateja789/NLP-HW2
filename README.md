# CS5760 — NLP Homework 2 (Spring 2026)

## 👤 Student Information

**Name:** KATTA SIVA TEJA
**Student ID:** 700774274
**Course:** CS5760 — Natural Language Processing

---

## 📌 Project Overview

This repository contains my solutions for **Homework 2** in NLP.
The assignment focuses on probabilistic models, evaluation metrics, and ethical considerations in NLP systems.

The work includes:

* Naive Bayes text classification with **Laplace smoothing**
* Analysis of **harms in automated classification**
* Bigram Language Model probability calculations
* Handling **zero-probability problems** in language models
* **Backoff model** reasoning for unseen trigrams
* Computing **precision, recall, macro-average, and micro-average**
* Python implementations for evaluation metrics and language modeling

---


## 🧠 Key Concepts Covered

### 1️⃣ Naive Bayes Classification

Used probabilistic reasoning with add-1 smoothing to classify a short document.
The posterior probability for the **negative class** was higher, so the text was labeled **Negative**.

---

### 2️⃣ Harms of Classification Systems

This assignment discusses real risks in NLP:

* **Representational harm:** Models reinforcing stereotypes
* **Censorship risk:** Toxicity systems suppressing identity-related speech
* **Dialect bias:** Models performing worse on varieties like AAE or Indian English due to dataset imbalance

---

### 3️⃣ Bigram Language Models

Sentence probability computed as:

[
P(w_1…w_n)=\prod_{i=2}^{n} P(w_i|w_{i-1})
]

Observed that unseen bigrams cause probability to collapse to zero.
This motivates smoothing or backoff strategies.

---

### 4️⃣ Backoff Models

When trigram counts are zero, the model backs off to bigram probabilities.
This ensures unseen sequences still receive meaningful probabilities.

---

### 5️⃣ Evaluation Metrics

From a confusion matrix, the following were computed:

* **Precision and Recall per class**
* **Macro-average** (treats all classes equally)
* **Micro-average** (weighted by frequency)

In single-label multi-class classification:
[
\text{Micro Precision} = \text{Micro Recall} = \text{Accuracy}
]

---


## 🛠 Requirements

This project only uses the Python standard library and NumPy.

Install NumPy if needed:

```bash
pip install numpy
```
