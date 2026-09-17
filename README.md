# 🎬 Movie Recommendation System

A content-based movie recommendation system built using **Python, Machine Learning, and Natural Language Processing (NLP)**. This project recommends movies based on similarities in their genres, taglines, and overviews.

## 📌 Project Overview

The Movie Recommendation System analyzes movie information and uses Natural Language Processing to identify similarities between movies.

When a user selects a movie, the system uses its textual features to find and recommend similar movies.

The project uses TF-IDF Vectorization to convert movie text into numerical features and cosine similarity to measure similarity between movies.

## 🚀 Key Features

* Content-based movie recommendation.
* Text preprocessing and feature engineering.
* NLP-based feature extraction using TF-IDF.
* Similarity-based movie recommendations.
* Pre-trained TF-IDF vectorizer and similarity data saved using Pickle.
* Movie dataset containing more than 45,000 records.

## 🛠️ Technologies Used

| Technology       | Purpose                                   |
| ---------------- | ----------------------------------------- |
| Python           | Programming language                      |
| Pandas           | Data loading and preprocessing            |
| NumPy            | Numerical operations                      |
| Scikit-learn     | TF-IDF vectorization and machine learning |
| NLP              | Processing movie text features            |
| Matplotlib       | Data visualization                        |
| Seaborn          | Data visualization                        |
| Pickle           | Saving trained objects and processed data |
| Jupyter Notebook | Development environment                   |

## 🧠 Machine Learning & NLP Concepts

### 1. Data Preprocessing

The original movie dataset contains information such as movie titles, genres, taglines, overviews, popularity, and ratings.

The project processes the movie data and prepares textual features for recommendation.

### 2. Feature Engineering

The following textual information is combined into a `tags` column:

* Genres
* Tagline
* Overview

This combined text represents the content of each movie.

### 3. TF-IDF Vectorization

TF-IDF (Term Frequency–Inverse Document Frequency) converts movie text into numerical vectors.

The project uses a TF-IDF vectorizer with a maximum of 50,000 features.

### 4. Cosine Similarity

Cosine similarity measures how similar two movie vectors are.

Movies with similar textual features can receive higher similarity scores and become recommendation candidates.

## 🔄 Project Workflow

```text
Movie Dataset
     ↓
Data Cleaning
     ↓
Text Feature Engineering
     ↓
Combine Genres, Tagline & Overview
     ↓
Create Tags Column
     ↓
TF-IDF Vectorization
     ↓
Numerical Feature Matrix
     ↓
Cosine Similarity
     ↓
Recommend Similar Movies
```

## 📂 Dataset

The project uses a movie dataset containing information about movies and their textual descriptions.

### Original Dataset

* File: `movies (1).csv`
* Rows: 45,466
* Columns: 24

### Processed Dataset

* File: `df.pkl`
* Rows: 45,447
* Columns: 7

Processed columns:

```text
title
popularity
genres
tagline
vote_average
overview
tags
```

## 📁 Project Structure

```text
Movie-Recommendation-System/
│
├── Recommendation (1).ipynb
├── movies (1).csv
│
├── df.pkl
├── indices.pkl
├── tfidf.pkl
├── tfidf_matrix.pkl
│
└── README.md
```

## 💾 Saved Model Files

| File               | Description               |
| ------------------ | ------------------------- |
| `df.pkl`           | Processed movie DataFrame |
| `indices.pkl`      | Movie title index mapping |
| `tfidf.pkl`        | Trained TF-IDF Vectorizer |
| `tfidf_matrix.pkl` | TF-IDF feature matrix     |



### 2. Navigate to the Project Directory

```bash
cd Movie-Recommendation-System
```

### 3. Install Required Libraries

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```
## 🔍 Example Usage

```text
Input Movie:
Toy Story

Output:
Recommended Movies:
1. [Recommendation 1]
2. [Recommendation 2]
3. [Recommendation 3]
4. [Recommendation 4]
5. [Recommendation 5]
```

## 📈 Future Improvements

* Develop a web interface using Streamlit.
* Add movie posters and additional movie details.
* Improve recommendation quality using additional movie features.
* Add user-based personalized recommendations.
* Deploy the recommendation system as a web application.

## 🎯 Learning Outcomes

Through this project, I learned:

* Data cleaning and preprocessing using Pandas.
* Text feature engineering.
* Natural Language Processing fundamentals.
* TF-IDF vectorization.
* Similarity-based recommendation systems.
* Saving and reusing trained machine learning objects.
* Building a machine learning project workflow.

## 👨‍💻 Author

**Jayjeet Singh**

B.Tech Mechanical Engineering Student | Machine Learning & Data Analytics Enthusiast


---

⭐ If you find this project useful, consider giving it a star!
