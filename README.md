# 🎬 Movie Recommender System

An interactive ML-based movie recommendation web app that suggests similar movies based on a user’s input using cosine similarity and content-based filtering. Built using Python, Streamlit, and movie metadata.

---

## 📌 1. Project Title / Headline
**Movie Recommender System – Content-Based ML Recommendation Engine**

A simple, responsive, and interactive recommendation dashboard that helps users find movies similar to the one they like.

---

## 📌 2. Short Description / Purpose
This project recommends top similar movies based on plot, cast, crew, and genre metadata. The system uses NLP-based feature extraction and similarity scores to generate relevant recommendations in milliseconds.

---

## 📌 3. Tech Stack

The project uses:

- 🐍 **Python** – Core programming  
- 📊 **Pandas** – Data handling  
- 🧮 **Scikit-Learn** – Vectorization + Cosine Similarity  
- 🎞 **TMDB / Movie Metadata Dataset**  
- 🌐 **Streamlit** – Web-based UI  
- 🌆 **TMDB API** (optional) – For fetching movie posters  

---

## 📌 4. Dataset Source

Common dataset sources:  
- **TMDB 5000 Movie Dataset (Kaggle)**  
- **Custom movie metadata (CSV)**  
- Fields used in the project:
  - Title  
  - Genres  
  - Cast  
  - Crew  
  - Overview  
  - Tags (combined features)

---

## 📌 5. Features / Highlights

### 🔹 Business Problem
Users frequently struggle to find similar movies manually. OTT apps often limit recommendations to trending content or platform-available titles.

Questions like:
- “If I liked *Spider-Man*, what similar movies exist?”
- “What movies share similar plot or cast?”
- “How to find recommendations based on movie metadata?”

…are solved using this ML-powered tool.

---

### 🔹 Goal of the Application
To provide:
- Accurate ML-based movie recommendations  
- Fast similarity search using vectorization  
- An intuitive Streamlit interface  
- Movie posters for a visual browsing experience  

---

### 🔹 Walkthrough of Key Features

#### **1. Search Bar**
Users type any movie name and the system suggests the closest match.

#### **2. Recommend Button**
On clicking "Recommend", the model fetches the top similar movies using cosine similarity.

#### **3. Movie Grid Display**
Recommended movies appear with:
- Poster  
- Title  

Everything displayed neatly in columns for easy browsing.

#### **4. Error Handling**
If a movie is not found, the system gracefully alerts the user.

---

## 📌 6. ML Model Process

### **1️⃣ Data Preprocessing**
- Remove missing values  
- Combine metadata into a single `tags` column  
- Clean text (lowercase, stemming)

### **2️⃣ Feature Vectorization**
```text
TfidfVectorizer / CountVectorizer
![App Preview](sample.png)
