# CS59000_06_Ethical_Artificial_Intelligence

# Ethical AI Fake News Detection System

This project implements a multi-model AI system to detect fake news ethically and accurately using a cleaned, balanced version of the [FakeNewsCorpus](https://github.com/several27/FakeNewsCorpus). It applies preprocessing, label filtering, text cleaning, and supports further modeling for classification.

---

## 📁 Dataset

- **Source:** [FakeNewsCorpus](https://github.com/several27/FakeNewsCorpus)
- **Used File:** `news_cleaned_big.csv`
- **Filtered Labels:** 
  - `fake`
  - `reliable`
  - `bias`
  - `clickbait`
  - `conspiracy`
  - `unreliable`

---

## 🧹 Preprocessing Steps

1. **Dropped unnecessary columns**  
   (e.g., `url`, `meta_keywords`, `authors`, etc.)
2. **Filtered by relevant labels**  
   Kept only samples from 6 target types.
3. **Filled missing titles** with `"Unknown title"`.
4. **Dropped remaining rows with NaN values**.
5. **Cleaned text** by:
   - Removing special characters
   - Lowercasing
   - Removing extra whitespaces
6. **Created new columns**:
   - `cleaned_content`
   - `cleaned_title`

---

## 📊 Exploratory Analysis

- Used Seaborn to visualize distribution of news types.
- Y-axis formatted in thousands (e.g., 100K).

---

## 📦 Requirements

Install dependencies:
```bash
pip install pandas seaborn matplotlib kagglehub
