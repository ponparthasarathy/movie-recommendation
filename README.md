# 🎬 Movie Recommendation System (Unsupervised Learning)

This project is a **content-based movie recommendation system** built using **Python**, **scikit-learn**, and **IMDb dataset**.  
It recommends movies based on **genre similarity** using **TF-IDF Vectorizer** and **Cosine Similarity**.

---

## 📌 Project Overview

The system takes a movie name as input and recommends similar movies by analyzing their genres.  
It uses **unsupervised learning** techniques to discover similarity patterns without using labeled data.

---

## 🧠 Machine Learning Approach

- **Type:** Unsupervised Learning  
- **Technique:** Content-Based Filtering  
- **Feature Extraction:** TF-IDF Vectorization  
- **Similarity Measure:** Cosine Similarity  

No supervised training or prediction is involved.

---

## 📂 Dataset

- Source: **IMDb Dataset (Kaggle)**
- Files used:
  - `title.basics.tsv` → Movie titles & genres
  - `title.ratings.tsv` → Ratings & vote counts

Only movies with more than **10,000 votes** are considered to ensure quality recommendations.

---

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Google Colab / Jupyter Notebook
- Streamlit (optional for UI)

---

## 🔄 How the Project Works

1. Load IMDb dataset
2. Filter only movies
3. Merge movie details with ratings
4. Remove low-vote movies
5. Convert genres into numerical vectors using TF-IDF
6. Compute cosine similarity between movies
7. Rank and recommend the most similar movies

---

## 🧪 Core Algorithm

### TF-IDF Vectorizer
- Converts movie genres into numerical feature vectors
- Assigns importance to genres based on frequency

### Cosine Similarity
- Measures similarity between movie vectors
- Higher cosine score = more similar movie

---

## 🧾 Recommendation Function

The system ranks movies based on **cosine similarity scores**, not ratings.

Ratings are used only for:
- Filtering low-quality movies
- Displaying information

---

## ▶️ How to Run the Project

### 1️⃣ Install dependencies
```bash
pip install pandas numpy scikit-learn
