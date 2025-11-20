# 🧠 Bag of Words (BoW) & TF-IDF — Scratch Implementation

This project demonstrates the **from-scratch implementation** of two fundamental text vectorization techniques — **Bag of Words (BoW)** and **TF-IDF (Term Frequency–Inverse Document Frequency)** — without relying on libraries like `scikit-learn`.  
It aims to build a strong conceptual understanding of how raw text is converted into numerical vectors for use in machine learning models.

---

## 🚀 Features

- Created a **custom vocabulary** from a corpus.  
- Implemented **Count-Based BoW** and **Binary BoW** representations.  
- Calculated **Term Frequency (TF)** and **Inverse Document Frequency (IDF)** manually.  
- Combined them to produce **TF-IDF vectors** from scratch.  
- Visualized BoW and TF-IDF as matrices using `pandas`.

---

## ⚙️ How It Works

1. **Preprocessing** — Tokenize the corpus and build a vocabulary of unique words.  
2. **BoW Construction** — Count how many times each vocabulary word appears in each sentence/document.  
3. **TF Calculation** — Normalize word counts by sentence length.  
4. **IDF Calculation** — Compute how unique each word is across the corpus.  
5. **TF-IDF Representation** — Multiply TF and IDF to get the final vector.

---

## 🧠 Concepts

| Technique        | Description                                                   |
|------------------|---------------------------------------------------------------|
| **Bag of Words** | Converts text into vectors based on word counts or presence.  |
| **TF-IDF**       | Scales word counts by how important/rare the word is overall. |

---

## 🧮 Example Output

### **Corpus:**

```
["I love data science", "Data science is fun"]
```

### **BoW Representation:**

| i | love | data | science | is | fun |
|---|------|------|----------|----|-----|
| 1 | 1    | 1    | 1        | 0  | 0   |
| 0 | 0    | 1    | 1        | 1  | 1   |

### **TF-IDF Representation:**

| i   | love | data | science | is   | fun  |
|-----|------|------|----------|------|------|
| 0.70 | 0.70 | 0.35 | 0.35 | 0    | 0    |
| 0    | 0    | 0.35 | 0.35 | 0.70 | 0.70 |

---

## 🧰 Tech Stack

- **Python 3.9+**  
- `nltk` — for tokenization  
- `pandas`, `numpy` — for tabular and numerical operations  

---

## 🎯 Learning Outcome

By building BoW and TF-IDF manually, this project reinforces:

- Core NLP preprocessing steps  
- Understanding of document vectorization  
- How libraries like scikit-learn’s `CountVectorizer` & `TfidfVectorizer` work internally  

---

## 📄 Author

**Vaibhav Pandey**  
_Data Science Enthusiast | NLP Learner | Building from first principles_


