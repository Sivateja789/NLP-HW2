# Bigram Language Model — Python Implementation

## 👤 Student Details

**Name:** KATTA SIVA TEJA
**Student ID:** 700774274
**Course:** CS5760 — Natural Language Processing

---

## 📌 Project Description

This project demonstrates how to build a simple **Bigram Language Model** in Python.
The objective is to learn word-to-word transition probabilities from a small training corpus and use those probabilities to evaluate how likely different sentences are.

The model estimates probabilities using **Maximum Likelihood Estimation (MLE)**.

---

## 🗂 Training Corpus

The model is trained on the following sentences:

```
I love NLP  
I love deep learning  
deep learning is fun
```

These sentences are used to learn word frequencies and transitions between consecutive words.

---

## ⚙️ What the Program Does

The Python script performs the following steps:

1. Reads the training sentences.
2. Computes **unigram counts** (frequency of each word).
3. Computes **bigram counts** (frequency of consecutive word pairs).
4. Calculates bigram probabilities using MLE:

[
$P(w_2 \mid w_1) = \frac{Count(w_1, w_2)}{Count(w_1)}$
]

5. Implements a function that calculates the probability of any sentence.
6. Tests the model on two sentences:

```
I love NLP
I love deep learning
```

7. Prints the probability of each sentence.
8. Displays which sentence the model prefers based on the higher probability.

---

## 📊 Program Output

When executed, the program will show:

* Unigram counts
* Bigram counts
* Bigram probabilities
* Sentence probabilities
* The sentence preferred by the language model

---

## 🧠 Concept Explanation

A **bigram language model** assumes that the probability of a word depends only on the previous word.
To calculate the probability of a full sentence, the model multiplies the probability of each bigram in that sentence.

The sentence with the higher final probability is considered more natural according to the model.

---

## ⚠️ Notes

* This implementation uses **MLE without smoothing**.
* If a bigram does not appear in the training data, its probability becomes **zero**, which causes the entire sentence probability to be zero.
* The project is designed for learning purposes to understand how statistical language models work.

