# Aviation Safety Reports – NLP Text Mining

This project applies Natural Language Processing (NLP) and Machine Learning to **aviation safety reports** in PDF format.  
The goal is to classify incident narratives (free-text descriptions) into predefined **event types** using a text classifier.

---

## Project Overview

- Input: PDF files containing aviation safety / incident reports (e.g. `acr_fatg.pdf`, `altdev.pdf`, `mechanic.pdf`, `nmac.pdf`, `wx.pdf`, etc.).
- Processing:
  - Extract raw text from PDFs using **PyPDF2**
  - Clean and preprocess report narratives
  - Convert text to numerical features using **TF-IDF**
- Model:
  - Train a **Linear Support Vector Classifier (LinearSVC)** using scikit-learn
  - Evaluate performance using `classification_report`
- Output:
  - A trained model that can **predict the event type** for a new narrative entered by the user.

---

## Repository Structure


```text
Aviation-Safety-Reports-Text-Mining/
│
├─ Aviation-Text-mining.ipynb     # Main Jupyter notebook for the project
├─ resources/
│   ├─ acr_fatg.pdf
│   ├─ altdev.pdf
|   |    '''''
│   ├─ mechanic.pdf
│   ├─ nmac.pdf
│   └─ wx.pdf
└─ README.md
```

---

## Technologies Used
Python

Pandas – data handling

PyPDF2 – PDF text extraction

scikit-learn – TF-IDF vectorization & LinearSVC model

Google Colab – experimentation environment
